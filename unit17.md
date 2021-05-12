# Unit 17: Star ratings, file uploads and data URLs

In this unit, we provide examples of implementation of common interactions in Vue.js, including star rating, and file upload. 

For file upload, we will learn how to upload a file to the server, and how to display image previews of files to upload. 

We will also learn that images can be represented via _data URLs_, which are strings that represent the bytes in images, encoded in such a way that they can be easily stored in the database, or uploaded via POST requests.  A typical data URL for an image begins with `data:image/jpeg;base64,` followed by the bytes of the image encoded in [base64](https://docs.python.org/3/library/base64.html) format. 
Data URLs enable us to convert images into strings, and thus, treat them just like any other simple data type, such as integers, floating point, etc, that can be send back and forth between browser and server via json and stored in the database.  See an example of this in the _adding images to contacts_ video.

## Resources

* [Code for star rating](https://bitbucket.org/luca_de_alfaro/star_ratings_2021/). Remember, you need to visit the `setup` controller to initialize the database once, before you can use the code.
* [Code to create a search bar](https://bitbucket.org/luca_de_alfaro/search_bar/)
* [Code for uploading files to the server](https://bitbucket.org/luca_de_alfaro/simple_file_upload/).
* [Code for uploading images with preview](https://bitbucket.org/luca_de_alfaro/upload_with_preview/).
* [Code to add images to contacts](https://bitbucket.org/luca_de_alfaro/contacts_with_images/).
* Information on [base64](https://docs.python.org/3/library/base64.html).
* Documentation on [data URLs](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URIs).
* Wikipedia page on [data URIs](https://en.wikipedia.org/wiki/Data_URI_scheme) (a.k.a. data URLs).
* Documentation on [FileReader](https://developer.mozilla.org/en-US/docs/Web/API/FileReader).
* Documentation on [XMLHttpRequest](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest).

## Videos

* [Implementing star ratings in Vue.js](https://youtu.be/IzkwpjE49Gs)
* [Implementing a search bar](https://youtu.be/TS6ToY5s0Eg).  This is a lower-quality video cut from a lecture.
* [Uploading files to the server](https://youtu.be/PaR4v7-OjXs) using Vue.js.
* [Uploading images with preview](https://youtu.be/5JrWHyGCS0w).
* [Adding images to contacts](https://youtu.be/VDPnflLmUxA).



