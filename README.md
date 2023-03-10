# Bank of Flatiron

Welcome to the Bank of Flatiron, where you can trust us with all your financial
data! Use the below gif as an example of how the app should function.

![demo](https://curriculum-content.s3.amazonaws.com/phase-2/phase-2-code-challenge-bank-of-flatiron/demo.gif)

> To view in VSCode, right click on the README.md file and select "Open Preview".

## Setup

1. Run `npm install` in your terminal.
2. Run `npm run server`. This will run your backend on port `8001`.
3. In a new terminal, run `npm start`. This will run your React app on port `8000`.

Make sure to open
[http://localhost:8001/transactions](http://localhost:8001/transactions) in the
browser to verify that your backend is working before you proceed!

## Endpoints

The base URL for the backend is: `http://localhost:8001`

### Endpoints for Core Deliverables

#### GET /transactions

Example Response:

```json
[
  {
    "id": 1,
    "date": "2019-12-01",
    "description": "Paycheck from Bob's Burgers",
    "category": "Income",
    "amount": 1000
  },
  {
    "id": 2,
    "date": "2019-12-01",
    "description": "South by Southwest Quinoa Bowl at Fresh & Co",
    "category": "Food",
    "amount": -10.55
  }
]
```

#### POST `/transactions`

Required Headers:

```js
{
  "Content-Type": "application/json"
}
```

Request Object:

```json
{
  "date": "string",
  "description": "string",
  "category": "string",
  "amount": number
}
```

Example Response:

```json
{
  "id": 1,
  "date": "2019-12-01",
  "description": "Paycheck from Bob's Burgers",
  "category": "Income",
  "amount": 1000
}
```

## Advanced Deliverables

These deliverables are not required to pass the code challenge, but if you have
the extra time, or even after the code challenge, they are a great way to
stretch your skills.

> Note: If you are going to attempt these advanced deliverables, please be sure
> to have a working commit with all the Core Deliverables first!

As a user, I should be able to:

- Sort transactions alphabetically by category or description.
- Delete a transaction which will remove it from the table and delete it from the backend.

### Endpoints for Advanced Deliverables

#### DELETE /transactions/:id

Example Response:

```json
{}
```
#   b a n k - o f - f l a t r i o n  
 