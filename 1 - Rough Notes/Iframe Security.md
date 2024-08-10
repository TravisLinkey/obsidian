
2024-08-09 10:53

Tags: [[Digital Payment]] | 

### Overview

Our web application is embedded in our clients site using an `iframe`. 

This makes it vulnerable to [[XSS]] attacks whereby the parent site could potentially inject scripts to run in out application. 

### The Soluion
Using a [[Content Security Policy]] we can ensure only trusted domains are embedding our application.

In addition, the [[Content Security Policy]] can be used to enforce httpswhich prevents insecure HTTP sources from loading resources. 

### References
- [[]]

