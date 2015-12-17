# Cloud_Project

For Documentation:  SecureUI/Documentation 

Youtube: https://youtu.be/y6yWZXkTELQ

SlideShare: http://www.slideshare.net/AkshayDharphale/mobile-security-solutions

This project aims at using android devices in place of CCTV cameras as they are cheaper alternatives. The device captures the picture,
uploads in a predefined interval (session) to the cloud.

The user can view all his uploaded images through a web interface and filter them using appropriate filters.
Components:

    Android Application - Secure
    Web Application - SecureUI
    Rest Backend service - RestService

AWS Service used:

    S3 - Stores the captured images.
    RDS - Store the user and session tables.
    EC2 - Virtual server that runs tomcat.
    EBS - Provides the block storage for the EC2 instance.
    CloudFront - Content delivery network to boost the image retrieval.

Deployment:
Secure.apk - Deployed to a compatible android phone. 
SecureUI.war - Deployed to a HTTP Server (Apache Tomcat) running in Amazon EC2. 
RestService.war - Deployed to a HTTP Server (Apache Tomcat) running in Amazon EC2.
