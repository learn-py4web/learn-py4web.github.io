# Unit 19: Deploying your App to Google Appengine and Google Cloud SQL

In this Unit we cover how to host your app on Google Appengine, with data stored in Google SQL.  This gives you an extremely scalable, and secure, hosting for your application. 

## Resources

* [Installation of Google Cloud SDK](https://cloud.google.com/sdk/docs/install).  You need to install these tools. 
* [Google Appengine Python 3 documentation](https://cloud.google.com/appengine/docs/standard/python3/).
* [Google Cloud SQL documentation](https://cloud.google.com/sql/docs/).
* [MySQL 5.7 documentation](https://dev.mysql.com/doc/refman/5.7/en/).

## Code

* You need to be running a version of py4web that includes the changes in the [luca-gcloud](https://github.com/lucadealfaro/py4web/tree/luca-gcloud) branch.  I think the py4web maintainers will merge the [PR](https://github.com/web2py/py4web/pull/539) soon, after that, you can simply update your py4web. 
* [google_cloud_example app](https://bitbucket.org/luca_de_alfaro/google_cloud_example/): This is the app we upload to the cloud (the README.md is important, and so are the details in `commons.py` and `settings.py`).

## Videos

* [Part 1: Creating the cloud project and configuring cloud OAuth login](https://drive.google.com/file/d/1QhBs1UZhJ8UoGVZbCQ6K6J0hh-3hwydD/view?usp=sharing).
* [Part 2: Configuring your app for OAuth login](https://drive.google.com/file/d/1CovGSCQeJWPyfVHnf2pvMSh-t72QZwYM/view?usp=sharing).
* [Part 3: Configuring the database connection](https://drive.google.com/file/d/12HOWBTMAw1FjOm9jU9UbgMwK6pujcMKb/view?usp=sharing).
* [Part 4: Creating and configuring the database](https://drive.google.com/file/d/1IXwr5DSBSYMAEHK6cPqEsEWKtWAulENz/view?usp=sharing).
* [Part 5: Deploying your app](https://drive.google.com/file/d/1thUcj2HczBq7bXf2TrhzssELPVOf1xrq/view?usp=sharing).