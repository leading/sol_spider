# sol_spider 
Monitor new tokens, transactions, and transaction pools on Solana.  
If you find it useful, please give it a star!!

Project Architecture

# Project Architecture
```
solana_newtoken_bot
├─ README.md
├─ swagger
│  └─ swagger.js  // API documentation
├─ utils
│  ├─ common
│  │  └─ common.js // Common utility methods
│  └─ blackchain
│     ├─ sol
│     │  ├─ sol_utils.js  // Solana related methods
│     │  ├─ transactionSender.js
│     │  ├─ getSignature.js
│     │  ├─ wait.js
│     │  ├─ pumpswap.js
│     │  └─ pupmswapUtils // Pump trading methods
│     │     ├─ utils.js
│     │     └─ constants.js
│     ├─ bsc
│     └─ eth
├─ app.js
├─ package.json
├─ service
│  ├─ bsc
│  ├─ sol
│  │  ├─ connect.js // RPC connection
│  │  ├─ monitor.js
│  │  └─ deal.js
│  └─ eth
├─ api
│  ├─ bsc
│  ├─ eth
│  └─ sol
│     ├─ sol_api.js // Solana API
│     └─ swagger
│        └─ swagger_sol_api.js  // API documentation config
├─ config
│  ├─ config.js
│  └─ config.prod.js // Production environment
├─ public
├─ db
│  ├─ db.js
│  ├─ pump_kline.js
│  ├─ insert_pump_token.js
│  ├─ test_mint_increase.js
│  └─ insert_raydium_newpool.js
├─ envtest
├─ test
├─ ws
│  └─ webSocketService.js  // WebSocket service
└─ sql
   └─ newtoken.sql  // Database structure SQL

```

# Runtime Version (Reference)
```
node V18.17.0
npm  V10.3.0
```
# How to Run
```
1. Rename the envtest file to .env
2. Configure the relevant parameters
3. npm install # Install dependencies
4. node app.js # Start the project
```

# API Documentation
```
After starting the project, open your browser:
http://127.0.0.1:18001/docs/
```

# Thanks for Your Support
```
If this project is useful for you and you need it, please contact me on Discord: hahha
```