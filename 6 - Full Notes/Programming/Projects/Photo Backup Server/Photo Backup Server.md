
Tags: [[Personal Projects]] 

### Overview

A Project I am working on to backup my personal photos to S3. Later I will extend this to include friends and family.

### Problems
1. I need to upload mutli-part/formData and it seems like API gateway (HTTPS) doesn't allow that.

### Solutions
1. Instead, use [[S3]] [[Presigned URLs]] to handle uploading the objects to S3. This does not require special headers or content types. 
2. Simply generate the presigned URLs and send Binary formatted data in a POST request to the URL, S3 will upload the file.

### References
[API Gateway FormData]()
