
2024-07-05 11:49

Tag:  [[Digital Checkout]]

## Overview


### Observations

- TP Display call is returning `isPaymentMethodCollected` boolean in display call to determine, on the front end, if a payment still needs to be captured
	- Digital Payment is using PaymentStatus === PENDING to determine if a payment needs fulfilled (Checking the Auth records)


### Requirements

- [ ] Create an endpoint to return the `CheckoutSession` status.
	- [ ] Determine exactly how to do this
	- [ ] Idea: check if Captures exist, check for a remaining balance.
- [ ] Show Alert on frontend when checkout session is complete

## References:

