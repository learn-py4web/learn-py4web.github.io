# Unit 8: Creating database tables, and using forms to insert/edit/view/delete data

In this unit, we learn how we can create simple database tables, and how we can use py4web and its forms to insert, view, edit, and delete data from the database. 

## Resources

* [The Database Abstraction Layer](https://py4web.com/_documentation/static/en/chapter-07.html), and in particular, 
    * the [Table constructor](https://py4web.com/_documentation/static/en/chapter-07.html#table-constructor) to create a new table; 
    * the [Field constructor](https://py4web.com/_documentation/static/en/chapter-07.html#field-constructor) to declare a table field. 
* [Field validators](http://web2py.com/books/default/chapter/29/07/forms-and-validators#Validators) in the web2py documentation.
* [Internationalization](https://py4web.com/_documentation/static/en/chapter-11.html), using the `T` operator. 
* [Learning forms on the MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms) contains good introductory material on HTML forms. 
* [Typical GET vs POST request processing](https://docs.google.com/presentation/d/1Q-HMRhR4BYkoIXy1cfVE9CP4jM1VeZrgvoLg3hppmYQ/edit?usp=sharing)

## Code

* [code for Creating a simple database table](https://github.com/learn-py4web/lecture_table_form). 
* [Code for A first simple form](https://github.com/learn-py4web/simple_form).
* [Code for An attack to the simple form](https://github.com/learn-py4web/simple_form_attacker).
* [Code for Form processing with py4web](https://github.com/learn-py4web/lecture_py4web_forms).

## Videos

* [Creating a simple database table](https://youtu.be/QMiwm0ZTEAA).
* [A first, simple, form](https://youtu.be/3nkdtnvFfdw).
* [An attack to the simple form](https://youtu.be/qvWVFy8pRxY).
* [Form processing with py4web](https://youtu.be/_prMUT6EpUc).

## Note

Compared to the recorded lecture, the [code for form processing with py4web](https://github.com/learn-py4web/lecture_py4web_forms) changed in one important respect.  The rule is this.  Suppose we create a URL signer `url_signer`.  Then: 

    Whenever `url_signer` is used in a template, we must include `url_signer` in the `@action.uses`. 

Example:

```
@action('index')
@action.uses('index.html', url_signer, db, auth.user)
def index():
    ...
```

This makes sense, as the fixtures are the things that should be "in place" before the page is processed.  More in detail, `url_signer`, to sign the URL, needs a key that is in the session.  In the `on_request` method, the URL signer generates the key it needs to sign the URLs.  Hence, we must list the `url_signer` in the fixtures, to ensure that the signing key has been produced before the template is processed. 
