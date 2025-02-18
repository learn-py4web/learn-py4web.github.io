# Unit 19: Storing files in Google Cloud Storage

It's all very good to be able to upload files, but the problem is, what should we do with the uploaded files? 

One may think, of course, we can just put them in the file system.  But this does not work.  As we have seen in [Unit 6](unit6.md), in a scalable web server there is not one, but potentially many servers, which are brought up and down on demand.  And for this reason, in the cloud deployment strategy we will present, web servers typically do not come with modifiable file systems.  Cloud web servers typically have read-only file systems, so that they are easy to duplicate and clone. 

If not in the file system, then we can consider using for uploaded files the same solution we use for all other data, namely, the database. 
In principle this works, and this works in practice also for small files, such as small thumbnail images. 
But this is very wasteful for large files, as the cost of database storage, typically in fast flash memory attached to a high-capacity dedicated host, is quite high. 

So the solution is to upload files to a blob store, such as [Amazon S3](https://aws.amazon.com/s3/) or [Google Cloud Storage](https://cloud.google.com/storage/).  In this unit, we pursue the latter solution. 

When a user wants to upload a file, this is what happens: 

1. The JavaScript in the browser asks the server for a signed URL to upload the file to Google Cloud Storage (GCS). 
2. The server replies with a signed URL to upload the file to a randomly-named blob in GCS. 
3. The JavaScript uploads the file to said blob. 
4. The JavaScript notifies the server that the upload succeeded. 
5. The server stores the name, type, size of the uploaded file, along with the blob used to store it in GCS. 

We show how to implement a complete app, including file deletion and download. 

## Resources

* [Google Cloud Storage](https://cloud.google.com/storage/).
* [NQGCS](https://bitbucket.org/luca_de_alfaro/nqgcs/), the package we use to access GCS from the server. 

## Code

* [GCS file storage](https://github.com/learn-py4web/gcs_file_storage).  See the setup video and the README.md file for instructions. 

## Videos

* [Part 1: The goal](https://youtu.be/wT_r2Oz-66c).
* [Part 2: Setup](https://youtu.be/tzrxFQZSZ1Q).
* [Part 3: The database](https://youtu.be/5vJ3M6NPvD4).
* [Part 4: The server](https://youtu.be/4eRQIcWN_3o).
* [Part 5: The client](https://youtu.be/EqrGKq76SxQ).


