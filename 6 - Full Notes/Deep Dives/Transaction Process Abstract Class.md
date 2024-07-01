
2024-06-09 13:15

Tag: [[Design Patterns]] | [[Strategy Pattern]] | [[6 - Full Notes/Professional/Job_Search/2024/Companies/ServiceCore/Interview]]

## Overview

The Transaction Process handles payment actions for various [[PSP]]s. The actions taken for these PSPs is very similar, the only difference is the business logic for each PSP.

This was a great opportunity to employ the [[Strategy]] pattern for encapsulating the logic that is shared using an [[Abstract Class]]. This enhanced the reusability and extendability of our code, while reducing the testing surface and mitigating potential bugs.

Now, as new PSPs are introduced, we have a well defined structure to the code which enhances the readability. As an added benefit, this design pattern reduces the time for onboarding new engineers when trying to understand the codebase.

