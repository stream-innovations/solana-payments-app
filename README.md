# **Stream**Payments App

This project allows Shopify and Medusa (developer construction) merchants to accept crypto through their shopify medusa store, and customers to purchase products using cryptocurrecies and USDC and EURC stablecoins.

[Visit Documentation](https://commerce.docs.streampayments.app)

[Test Payment flow](solanatest8.myshopify.com) 

[Test Merchant Flow](merchant-staging.streampayments.app)

# Local Development

## Dependencies

These steps will get you up and running with a local dev environment, and you can later setup these environments for production

-   Dependencies

    -   Docker Desktop
    -   Mysql

-   Keys

    -   Gas Keypair
        -   .env.dev in backend serverless
    -   [Helius API key](https://www.helius.dev)
        -   .env.dev in backend serverless

-   Dev Certs

    -   [Follow this guide](https://blog.simontimms.com/2021/10/12/serverless-offline-https/)
    -   included sample dev certs in backend-serverless & mock-shopify-serverless, must proceed to safety on google chrome

## Commands

Installation:

```
git clone https://github.com/stream-innovations/stream-payments-app
yarn install
yarn setup:env
```

Once the dependencies are all setup, env variables are set:

```
yarn dev
yarn seed
```

```
node --loader ts-node/esm scripts/nft-setup.ts
```

## Testing

Use these links to test out the local development flow

[Local Merchant UI](https://localhost:4004/install)

[Local Payment Simulation](https://localhost:4004/payment)
