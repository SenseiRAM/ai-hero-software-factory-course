# Cadence

Cadence is a platform for selling and taking online video courses. This glossary sets the words used for its concepts, both in the product and in the code.

## Language

### People

**Student**:
A person who buys and takes courses.
_Avoid_: Learner, Customer, Buyer

**Reviewer**:
The Admin who reviews a Refund Request.
_Avoid_: Resolver, Approver

### Refunds

**Refund**:
Money returned to a Student for one purchase of a course. Once a Refund is made, the Student can no longer access that course.
_Avoid_: Cancellation, Reversal, Chargeback

**Refund Request**:
A Student's request for a Refund on one purchase, with their reason. A Reviewer reviews every Refund Request.
_Avoid_: Refund (when nothing has been approved yet), Cancellation request

**Review**:
A Reviewer's decision on a Refund Request, which ends in Approved or Declined.
_Avoid_: Resolve, Resolution

**Pending**:
The state of a Refund Request that hasn't been reviewed yet.
_Avoid_: Requested, Open

**Approved**:
The outcome of a Refund Request that leads to a Refund.
_Avoid_: Accepted, Granted

**Declined**:
The outcome of a Refund Request that leads to no Refund.
_Avoid_: Rejected, Denied

**Refund Amount**:
The money a Refund returns: what the Student paid for that purchase.
_Avoid_: Reversal amount, list price

### Refund Eligibility

**Refund Eligibility**:
Whether a purchase can get a Refund Request right now. A purchase is either eligible or not eligible.
_Avoid_: Cancellation offer, can cancel

**Refund Window**:
The span of calendar days, counted from the purchase date, during which a purchase can be eligible.
_Avoid_: Cancel window, Cancellation period

**Watch Limit**:
The amount of a course's video a Student can watch before their purchase stops being eligible.
_Avoid_: Watched too much, Max watched hours

**Completion Limit**:
The share of a course's lessons a Student can complete before their purchase stops being eligible.
_Avoid_: Cancel completion limit

**Claimed Seat**:
A seat from a team purchase that a team member has taken. A Claimed Seat is never eligible.
_Avoid_: Redeemed coupon (when talking about refunds)

### Outside Cadence

**Chargeback**:
A dispute the cardholder raises with their bank or card issuer, outside Cadence. It is not a Refund.
_Avoid_: using it for any part of the Refund flow
