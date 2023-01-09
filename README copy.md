# Academy Serverless Framework

Serverless application for user creation, card assignment (gold or classic) and gifts.
When creating a user, the parameters chosen are taken into account to differentiate the type of card and gift granted.


Lambdas:

- create-client: load clients with ID, name, surname and date of birth. You should only allow adults up to 65 years of age
- create-card: grants a credit card (Classic if under 45 and Gold if older) generating number, expiration date and security code.
- create-gift: assign a birthday gift according to the season in which it falls, varying between a sweatshirt if it is autumn, a sweater if it is winter, a shirt if it is spring and a t-shirt if it is summer.

## Body

Required fields:

```javascript
{
    "dni":"0303456",
    "name": "Pepe",
    "lastName": "Argento",
    "birth": "1992-06-09"
}
```
