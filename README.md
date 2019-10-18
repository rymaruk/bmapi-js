![](https://login.bm.parts/static/img/bm_logo_.svg)

# BusMarket API JS client


```
⚠ UNDER CONSTRUCTION ⚠
This is a short version of the library BusMarket API JS client.
```
For a comprehensive list of examples, 
check out the [API documentation](https://developer.bm.parts/).


### Installation

~~npm install bmapi --save~~

### Overview

Every resource is accessed via your BmApi instance:

```js
const BmApi = require('bmapi');
const myBmApi = new BmApi('<your_token>');
```

Using TypeScript:

```typescript
import BmApi = require("bmapi");
const myBmApi = BmApi('<your_token>');
```

### Engine
Every resource method returns a promise.
For example, let's get list of products:

```js
const BmApi = require('bmapi');
const myBmApi = new BmApi('<your_token>');
(async() => {
  const response = await myBmApi.search.products({q: '115906'});
  console.info(response.data);
})();
```

### Documentation

Documentation is available at https://developer.bm.parts
