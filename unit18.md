# Unit 18: File uploads and data URLs

In this unit, we will learn how to upload a file to the server, and how to display image previews of files to upload. 

We will also learn that images can be represented via _data URLs_, which are strings that represent the bytes in images, encoded in such a way that they can be easily stored in the database, or uploaded via POST requests.  A typical data URL for an image begins with `data:image/jpeg;base64,` followed by the bytes of the image encoded in [base64](https://docs.python.org/3/library/base64.html) format. 
Data URLs enable us to convert images into strings, and thus, treat them just like any other simple data type, such as integers, floating point, etc, that can be send back and forth between browser and server via json and stored in the database.  See an example of this in the _adding images to contacts_ video.

## Resources

* Information on [base64](https://docs.python.org/3/library/base64.html).
* Documentation on [data URLs](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URIs).
* Wikipedia page on [data URIs](https://en.wikipedia.org/wiki/Data_URI_scheme) (a.k.a. data URLs).
* Documentation on [FileReader](https://developer.mozilla.org/en-US/docs/Web/API/FileReader).
* Documentation on [XMLHttpRequest](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest).

## Code

* [Code for uploading files to the server](https://github.com/learn-py4web/simple_file_upload).
* [Code for uploading images with preview](https://github.com/learn-py4web/upload_with_preview).
* [Code to add images to contacts](https://github.com/learn-py4web/contacts_with_images).

## Videos

* [Uploading files to the server](https://drive.google.com/file/d/1v5iOhw-GYFVd90pjHBtLgkvkvieY5zs9/view?usp=sharing) using Vue.js.
* [Uploading images with preview](https://drive.google.com/file/d/1zQJ1DZAlRobOvf9wYCpj7lsnsLzKCVtb/view?usp=sharing).
* [Adding images to contacts](https://drive.google.com/file/d/1ccBp4iZOf9dEoIviVT-wSUR2Rtc2yOq_/view?usp=sharing).

