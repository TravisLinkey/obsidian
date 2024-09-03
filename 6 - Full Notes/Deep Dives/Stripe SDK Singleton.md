
2024-06-09 13:15

Tag: [[Design Pattern]] | [[Singleton Pattern]] | [[3 - Tags/Interview|Interview]]

## Overview

The Stripe SDK is initialized using a ClientId which is specific to the caller making the request. In our case, it is the client application that is calling our backend. This client id is coming from the Okta token that is sent in on the header of the request. 

The issue is, we have a Lambda that is initializing our Stripe client and may reuse that initialized Stripe Client if the lambda is executed with sequential requests. 

What we needed to do was create a Stripe Client that would be able to be reused if the caller had the same ClientId within the context of the request. If not, we would reinitialize a new Stripe Client. To do this, we created a singleton class that could be reused, but when a SDK call was made, we would pass in the Client Id and ensure that it matched the Client Id that initialized the Stripe Client.

