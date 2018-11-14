# Assignment #1

## Getting Started

### Prerequisites

Https Server is only valid for limited time. To regenerate, `cd https` and run the following:

```commandline
openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem
```

### Running Server
#### To run server in staging mode:

```commandline
NODE_ENV=staging node index.js
```

Http is run on port [3000](http://127.0.0.1:3000) and Https is run on port [3001](https://127.0.0.1:3001)

#### To run server in production mode:

```commandline
NODE_ENV=production node index.js
```

Http is run on port [5000](http://127.0.0.1:5000) and Https is run on port [5001](https://127.0.0.1:5001)

### RESTful JSON API

Route|Outcome
---|---
/ping|200 status code if website is up
/hello|prints a message
