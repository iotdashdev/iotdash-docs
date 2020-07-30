---
description: >-
  The page describes the development & testing procedures for the
  frontend(react)
---

# Dev & Test

## Install dependencies

Install & update dependencies using with [npm](https://www.npmjs.com/)

```
$ npm install 
```

## Check global variable

Under the project directories, open .env file. Make sure your backend-api is valid.

```bash
REACT_APP_BACKEND_API_KEY=https://iotdash-backend-dev.herokuapp.com/api
REACT_APP_PORT=3000
```

{% hint style="info" %}
When development, you can change the **REACT\_APP\_BACKEND\_API\_KEY** to your local backend api, such as http://localhost:5000

Before deployment, change the **REACT\_APP\_BACKEND\_API\_KEY** to your deployed backend api.
{% endhint %}

## Start the script

```bash
npm start
```



