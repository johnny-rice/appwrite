const sdk = require('node-appwrite');

const client = new sdk.Client()
    .setEndpoint('https://<REGION>.cloud.appwrite.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const account = new sdk.Account(client);

const result = await account.create(
    '<USER_ID>', // userId
    'email@example.com', // email
    '', // password
    '<NAME>' // name (optional)
);
