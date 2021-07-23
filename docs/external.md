# Serving Research Data Externally

You can use a static website to serve data publicly to collaborators or services that need to see the data via http. A common example of this is hosting tracks for the UCSC Genome Browser. 

To set one up, first get an account on ITS's [Spinup](http://spinup.internal.yale.edu) service. After that, follow their [instructions on creating a static website](https://yaleits.atlassian.net/wiki/spaces/spinup/pages/905969895/How+do+I+use+a+Spinup+static+website), giving it an appropriate website name. Then use an [S3 transfer tool](https://yaleits.atlassian.net/wiki/spaces/spinup/pages/829292599/How+do+I+use+a+Spinup+S3+bucket) like AWS CLI, CrossFTP, or Cyberduck to transfer your files.

!!! info
    There will be a cost for storing the data (a few cents per GiB per month), which you can use Yale charging instructions to pay for.

# Attaching Globus to S3

The YCRC supports creating Globus S3 Endpoints. At this time, users cannot self-serve new Globus S3 Endpoints. To request a Globus S3 Endpoint, please [contact YCRC](https://docs.ycrc.yale.edu/#web-and-email-support). Please include in your request:

- Bucket name
- The [Amazon Region](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions) for that bucket
- An initial list of Yale NetID(s) who should be able to access the bucket
- Please DO NOT send us the Amazon login credentials through an insecure method such as email or our ticketing system.

After Globus S3 Endpoint creation, the user(s) will be able to further self-serve their own access controls using Globus.
