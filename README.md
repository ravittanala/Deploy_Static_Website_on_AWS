# Deploy_Static_Website_on_AWS
Creation of a Static Website using AWS s3: In this project we are using Amazon S3, CloudFront and IAM services.

Amazon S3 (Simple Storage Service) is a scalable, high-speed, low-cost web-based service designed for online backup and archiving of data and application programs. It allows to upload, store, and download any type of files up to 5 TB in size. This service allows the subscribers to access the same systems that Amazon uses to run its own web sites. The subscriber has control over the accessibility of data, i.e. privately/publicly accessible.

CloudFront is a CDN (Content Delivery Network). It retrieves data from Amazon S3 bucket and distributes it to multiple datacenter locations. It delivers the data through a network of data centers called edge locations. The nearest edge location is routed when the user requests for data, resulting in lowest latency, low network traffic, fast access to data, etc.

  How AWS CloudFront Delivers the Content?
  AWS CloudFront delivers the content in the following steps.

  Step 1 − The user accesses a website and requests an object to download like an image file.

  Step 2 − DNS routes your request to the nearest CloudFront edge location to serve the user request.

  Step 3 − At edge location, CloudFront checks its cache for the requested files. If found, then returns it to the user otherwise does     the following −

  First CloudFront compares the request with the specifications and forwards it to the applicable origin server for the corresponding     file type.

  The origin servers send the files back to the CloudFront edge location.

  As soon as the first byte arrives from the origin, CloudFront starts forwarding it to the user and adds the files to the cache in the   edge location for the next time when someone again requests for the same file.

  Step 4 − The object is now in an edge cache for 24 hours or for the provided duration in file headers. CloudFront does the following −

  CloudFront forwards the next request for the object to the user’s origin to check the edge location version is updated or not.

  If the edge location version is updated, then CloudFront delivers it to the user.

  If the edge location version is not updated, then origin sends the latest version to CloudFront. CloudFront delivers the object to the   user and stores the latest version in the cache at that edge location.

IAM: AWS Identity and Access Management (IAM) enables us to securely control access to AWS services and resources for the users. Using IAM, we can create and manage AWS users and groups and use permissions to allow and deny their permissions to AWS resources.


Supporting Files:

The Files and Folders included are: 

index.html - The Index document for the website.

Documents for different areas in the Website.
post-CD.html
post-CI.html
post-CI-CD-Practice.html
post-DevOps.html
Post-Tools.html

/img - The background image file for the website.
/vendor - Bootssrap CSS framework, Font, and JavaScript libraries needed for the website to function.
/css - CSS files for the website.


