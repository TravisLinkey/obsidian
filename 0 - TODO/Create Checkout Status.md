
2024-07-05 11:49

Tag:  [[Digital Checkout]]

## Overview


### Observations

- TP Display call is returning `isPaymentMethodCollected` boolean in display call to determine, on the front end, if a payment still needs to be captured
	- Digital Payment is using PaymentStatus === PENDING to determine if a payment needs fulfilled (Checking the Auth records)


### Requirements

- [x] Create an endpoint to return the `CheckoutSession` status.
	- [x] Determine exactly how to do this
        - Update the top-level record when a capture / refund takes place
	- [ ] Idea: check if Captures exist, check for a remaining balance.

- [ ] Show Alert on frontend when checkout session is complete


### Solution

- Use a top-level paymentStatus on CheckoutDAO which is updated any time a capture / refund takes place.
- The front end will check this paymentStatus to determine whether to render or not render the payment page.

#### Open Questions

- [ ] 

## References:

