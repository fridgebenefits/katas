**ADR 2 – Point-Of-Sale abstraction**

**STATUS:**
Accepted

**CONTEXT:**
Point-Of-Sale (POS)– there are two ways by which the sale will occur – (1) Smart Fridges (2) Kiosks. The sale can occur in the way of subscriptions or also we are allowing new customers to be able to buy or try meals at the Point-Of-Sale. For simplified implementation, we are requesting the Service-Agent at the POS to be help the customers to be able to use the one-time payment.

Our subscribed customers to be able to receive meals at the POS can have one of the following options – (1) one-time passcode sent via mobile and email for each meal or (2) QR code available as part of the customer profile to be able to scan at the POS

**DECISION:**
Payment functionality is made available at the POS. Each POS will include the payment system for customers to be able to buy the meals.

For Subscribed customers a decision has been made to use the QR code for simplifying the customer experience. Using the one-time passcode sent via mobile and email at the POS – adds complexity into the system by adding another use case to handle the lost pass code by customers and add a background process to generate one-time passcode for every meal.

**CONSEQUENCES:**
When a customer registers for the meal plan subscription, a unique QR code will be generated.
POS sale system should include the QR code scanner.

