Finding #1
Incomplete Documentation

Missing:
Project overview
Architecture
API documentation
Setup instructions
Build instructions
Test execution steps
Assumptions and limitations

Recommendation:
Provide a detailed README covering project setup, architecture, API endpoints and testing instructions.

Finding#2
Missing ID Generation strategy

Observations:
code can be null or empty.
Discount can be negative.
minBasketValue can be negative
Recommendation:
Use validation annotations:
@NotBlank
@DecimalMin(“0.0”)

Finding#3
Lombok @Data on Entiy
Severity : High
Location : core/domain/Coupon.java

Observation:
Using @Data on JPA Entities genrates equals(), hashCode(), and toString()

