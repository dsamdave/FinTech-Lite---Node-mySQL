# fintech-lite

I had an idea to build a basic digital bank.

## Disclaimer

All the code here may not exactly be _production ready_.

## Getting Started

1. You need to have [Node.js](https://nodejs.org/en/download) and [MySQL](https://dev.mysql.com/downloads/mysql/) installed.
2. Install project dependencies by running `npm install`.
3. Create a `.env` file in the root directory and add your databae details. It should have the following properties:

- DATABASE_HOST=
- DATABASE_USERNAME=
- DATABASE_PASSWORD=
- DATABASE_NAME=
- DATABASE_PORT=

4. Run the migrations to create database tables by running `npm run migrate`.
5. You can create two users by calling the `createUser` function in `app.js` with the `username` and `password` arguments. Something like this:

```
createUser('johndoe', 'doedoe').then(console.log).catch(console.log);
createUser('johnlol', 'lololo').then(console.log).catch(console.log)
```

This will generate records in both the `users` table as well as `accounts` table.

6. You can go ahead to test each transaction function.

### Note:

To run basic wallet functionalities, run the functions in `app.js`.
To run the card functions for debit and authorization, run the functions in `card.js`.

## Branches

## Contributions

### Feature Requests
