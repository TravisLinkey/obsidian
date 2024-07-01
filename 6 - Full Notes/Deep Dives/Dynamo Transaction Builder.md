
2024-06-09 13:15

Tag: [[Design Patterns]] | [[Builder Pattern]] | [[3 - Tags/Interview|Interview]]

## Overview

Due to the nature of our application, (creating financial transactions) there was a need to adhere to the [[ACID]] principle for transactions that were being created. Specifically, our transactions needed to be [[Atomicity]] so that they either all succeeded, or they all failed.

From a technical requirement standpoint, we needed to ensure that calls made to various PSPs were completed before we updated records in our database. This included updates to several records at a time (Capture records, payment records, etc). 

To acheive this, we needed to create a [[Builder]] class for [[DynamoDB]] client that would allow adding record updates to batch process that occurred as a transaction. The way this would work is, when any record needed to be created or updated, we would add this updated information to a list within the DynamoDB Client builder class, and only when the entire function had processed would we execute the batch updates.
