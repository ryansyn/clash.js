<div align="center">
  
  ![Logo](https://developer.clashofclans.com/front-bg-small.d355db.jpg)
  
  [![Npm](https://img.shields.io/npm/v/clash.js)](https://www.npmjs.com/package/clash.js)
  [![Downloads](![npm](https://img.shields.io/npm/dt/clash.js))](https://www.npmjs.com/package/clash.js)

</div>

### About

**clash.js** is a simple [Node.js](https://nodejs.org/en/) module that allows you to easily interact with the [Clash of Clans API](https://developer.clashofclans.com/#/)
  - Object-oriented
  - Predictable abstractions
  - 100% coverage of API (striving for)

### Implementation
requires [Node.js](https://nodejs.org/en/) version 14.0.0 or newer
```sh-session
npm i clash.js
```
  
### Example
  
```js
const { Client } = require("./clash.js");
const client = new Client(process.env.COC_API_TOKEN);

(async () => {
  const player = await client.getPlayer("#ABC");
  
  console.log(`${player.getPlayerName} (${player.getPlayerTag})`);
})();
```
