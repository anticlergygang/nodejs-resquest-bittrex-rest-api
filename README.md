Find a dev: https://discord.gg/PKk3Xc4

Get your apikey and sceret from: https://bittrex.com/home/api

```javascript
const bittrex = require('nodejs-request-bittrex-rest-api');

bittrex.getmarkets().then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getcurrencies().then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getmarketsummaries().then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getticker(marketName).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getmarketsummary(marketName).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getmarkethistory(marketName).then(out => {
    console.log(out);
}).catch(err => {});

// tickInterval must be one of the following 'oneMin', 'fiveMin', 'thirtyMin', 'hour', or 'day'
bittrex.getticks(marketName, tickInterval).then(out => {
    console.log(out);
}).catch(err => {});

// type must be one of the following 'buy', 'sell', 'both'
bittrex.getorderbook(marketName, type).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getbalances(apikey, secret).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getbalance(apikey, secret, currency).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getdepositaddress(apikey, secret, currency).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.withdraw(apikey, secret, currency, quantity, address).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getorder(apikey, secret, uuid).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getorderhistory(apikey, secret, marketName).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getwithdrawalhistory(apikey, secret, marketName).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getdeposithistory(apikey, secret, marketName).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.buylimit(apikey, secret, marketName, quantity, rate).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.selllimit(apikey, secret, marketName, quantity, rate).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.cancel(apikey, secret, uuid).then(out => {
    console.log(out);
}).catch(err => {});

bittrex.getopenorders(apikey, secret, marketName).then(out => {
    console.log(out);
}).catch(err => {});
```