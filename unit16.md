# Unit 16: Building applications with Vue.js

In this unit, we will learn how to develop Vue applications that receive and send information from/to the server.  

Our main example consists in a Vue app that manages a list of contacts.  The app (the page) will load the contacts from the server, visualize them, let the user add contacts, and delete them.  We will then see how to use Vue to enable editing the contacts in place. 

We also discuss how to implement navigation in Vue, that is, how to send the user to other pages when the user interacts with Vue-generated content. 

## Resources

* [Vue documentation](https://vuejs.org/v2/guide/installation.html).  In particular, look at: 
    * [The Essentials section](https://vuejs.org/v2/guide/installation.html) of the Vue guide. 
    * [Reactivity in depth](https://vuejs.org/v2/guide/reactivity.html): read this section to understand how Vue keeps the page in synch with the JavaScript, and to avoid common pitfalls in this. 

* [Bulma documentation](https://bulma.io/documentation/overview/).

* Watch the video on how to [debug Vue.js apps](howto2.md).

* Browser JavaScript documentation: 
    * [createElement](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement) documentation. 
    * [window.location](https://developer.mozilla.org/en-US/docs/Web/API/Window/location) documentation.

## Code

* [A contacts app in Vue.js](https://github.com/learn-py4web/lecture_vue_contacts).
* [Editing contacts in place](https://github.com/learn-py4web/lecture_vue_contacts_edit_in_place).
* [Vue reactivity](https://github.com/learn-py4web/vue_reactivity); the last commit corresponds to the end of the class; look at previous commits to see the initial state. 
* [Code for the navigation in Vue app](https://github.com/learn-py4web/vue_navigation).  You need to look at the various [branches](https://github.com/learn-py4web/vue_navigation/branches) of this repository to find the various versions of the navigation code discussed in the video. 

## Videos

* [A contacts app in Vue.js](https://drive.google.com/file/d/1Mzoj6-IMbsouH4eKtuEToidfvToWJyV8/view?usp=sharing) ([YouTube](https://youtu.be/Qh3xUZWsqR4)).
* [Editing contacts in place](https://drive.google.com/file/d/1-H7gZV-RCNIjR3mlj-0Ugs37Ycc1qGdK/view?usp=sharing) ([YouTube](https://youtu.be/gi7EDFLvXyA)). 
* [Reactivity](https://drive.google.com/file/d/1gfV9eL4GJCFFANBdqaUDqyuTlabMEMFk/view?usp=sharing) ([YouTube](https://youtu.be/4Rc_33ee9Yc)), or better, how to debug reactivity issues in Vue. 
* [URLs and Navigation in Vue](https://drive.google.com/file/d/1fhyzE7xMSUAOJtb42Tv6YuVwcKOlVWbK/view?usp=sharing) ([YouTube](https://youtu.be/AvqXmq3hwI4)).