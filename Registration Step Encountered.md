# Registration Step Encountered

Fire whenever a user encounters a new registration step.

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  event: 'Registration Step Encountered',
  ecommerce: {
    checkout: {
      actionField: {
        step: '<stepNumber>',
      },
      products: [{
        name: '<eventName>',
        id: '<eventId>',
        price: '<initialDonationAmount>',
        brand: '<brand>',
        category: '<category>',
        variant: '<variant>',
        quantity: 1,
     }]
   }
 },
 registrationFlow: {
   stepName: '<stepName>',
   stepNumber: '<stepNumber>',
   participantType: '<participantType>',
   fundraisingGoal: '<fundraisingGoal>',
   initialDonationAmount: '<initialDonationAmount>',
   teamRole: '<teamRole>',
   teamName: '<teamName>',
   discountCode: '<discountCode>'
 }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Progam individual is registering for|RFL, MSABC, ACS
|category|string|The platform used to register/donate (donate, events, p2p)|p2p
|discountCode|string|The discount code used by the individual, if any|Discount Code Goes Here
|fundraisingGoal|string|The fundraising goal set by the registrant|100, 200, 500
|initialDonationAmount|string|The initial donation amount of the registrant|100, 200, 500
|participantType|string|The type of individual participating|survivor, caregiver, participant, no response
|stepName|string|The name of the current step in the checkout flow|fundraising, team, contact, payment
|stepNumber|integer|The current step in the checkout flow|1,2,3,4
|teamRole|string|The role the registrant signed up as|captain, member, individual
|teamName|string|The name of the team the registrant joined|Testing team
|variant|string|Single vs recurring (ACS) and team fundraiser vs individual fundraiser (Blackbaud)|team, individual

## Registration steps
1. Fundraising
2. Fundraising
3. Team
4. Team
5. Contact
6. Contact
7. Payment
8. Payment
