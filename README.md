# API-Doc
Our API documentation can help you integrate your bot into SCARPS Bot List to do things like vote lock commands and reward your users!

# **Server Count API**
Update your bot's count.

**Javascript**

```js
const fetch = require("node-fetch")
fetch('https://botlist.scarps.club/api/auth/stats/:botid', {
    method: "POST",
    headers: { 
      Authorization: "YOUR_AUTH_TOKEN",
      "Content-Type": "application/json"
    },
    body: JSON.stringify({"server_count": 0}) // Replace this number with the server count
  }).then(response => response.text())
.then(console.log).catch(console.error)
```

# **Check Voted API**
Get an array of users who have voted for your bot.

**Javascript**
```js
const fetch = require('node-fetch');
fetch('https://botlist.scarps.club/api/auth/liked/:botid', { headers: { 'Authorization': "YOUR_VB_AUTH_KEY" } }).then(res => res.json()).then(data => {
  return console.log(data);
}).catch(console.error);
```
**Docs:** https://docs.scarps.club/
**List:** https://botlist.scarps.club
# Need help Join our **Discord** : https://discord.gg/XQhdYjzTrT 
