# Unit 20: Deploying your App to Google Appengine and Google Cloud SQL

In this Unit we cover how to host your app on Google Appengine, with data stored in Google SQL.  This gives you an extremely scalable, and secure, hosting for your application. 

## Resources

* [Installation of Google Cloud SDK](https://cloud.google.com/sdk/docs/install).  You need to install these tools. 
* [Google Appengine Python 3 documentation](https://cloud.google.com/appengine/docs/standard/python3/).
* [Google Cloud SQL documentation](https://cloud.google.com/sql/docs/).
* [MySQL 5.7 documentation](https://dev.mysql.com/doc/refman/5.7/en/).

## Code


* [google_cloud_example app](https://github.com/learn-py4web/google_cloud_example): This is the app we upload to the cloud (the README.md is important, and so are the details in `commons.py` and `settings.py`).

## Notes

* You need to be running a version of py4web that includes the changes in this [PR](https://github.com/web2py/py4web/pull/539).  **Update your py4web to the latest version to get them.**
* Google is everywhere... but especially in Los Angeles!  Don't do as I did in my video: **do not create the database in Oregon (us-west1); rather, choose Los Angeles (us-west2).** For some reason, Google appengine is not available in us-west1, and it is best to keep database and appengine in the same location, to reduce latency.
* The DB machine type I used is db-f1-micro, which is [$7.67 / month](https://cloud.google.com/sql/pricing#mysql-pg-pricing) at the time of writing.

## Videos

* [Part 1: Creating the cloud project and configuring cloud OAuth login](https://youtu.be/AeGXq3PaJDQ).
* [Part 2: Configuring your app for OAuth login](https://youtu.be/LiypQk4bP38).
* [Part 3: Configuring the database connection](https://youtu.be/ubl6In12aFc).
* [Part 4: Creating and configuring the database](https://youtu.be/4mCIdMr6mdw).
* [Part 5: Deploying your app](https://youtu.be/AHldkj1kyuI).