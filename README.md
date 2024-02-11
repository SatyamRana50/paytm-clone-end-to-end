
# Project Title

This project is a clone of the Paytm application developed using the MERN (MongoDB, Express.js, React.js, Node.js) stack. It provides functionalities similar to Paytm, including user authentication, wallet management, money transfer, and more.


## API Reference

#### create a new user

```http
  POST /api/vi/user/signup
```

| req body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `firstName` | `string` |  `firstName of user` |
| `lastName` | `string` |  `lastName of user` |
| `username` | `string` |  `username of user` |
| `password` | `string` |  `password of user` |

#### login to access your account

```http
  POST /api/vi/user/signin
```

| req body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `username` | `string` |  `username of user` |
| `password` | `string` |  `password of user` |

#### update profile

```http
  PUT /api/vi/user
```

| req body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `firstName` | `string` | firstName to be updated |
| `lastName` | `string` | lastName to be updated |
| `password` | `string` | password to be updated |

#### get the users by the filter keyword in their firstName or lastName

```http
  GET /api/vi/user/bulk/${filter}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `filter`      | `string` | filter to get the matching users |

#### get the accont balance of the user
```http
  GET /api/vi/account/balance/
```
#### transfer money to a friend
```http
  POST /api/vi/account/transfer/
```
| req body | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `amount` | `number` |  `amount to be sent in Rs.` |
| `to` | `string` |  `userId of friend to whom money to be send` |




## Authors

- [@SatyamChauhan](https://github.com/SatyamRana50)


## Demo

Insert gif or link to demo


## 🛠 Skills
React, NodeJs, ExpressJs, MongoDb


## Optimizations

- Performance Improvements: proper state management avoiding unnecessary rendering
- Code Splitting: Splitting large codebases into smaller, modular components can improve loading times and facilitate easier maintenance and debugging.
- Caching: Implementing caching mechanisms for frequently accessed data can reduce database queries and improve response times.
- Error Handling: Implementing robust error handling mechanisms, including proper logging and informative error messages, can improve troubleshooting and debugging.
- Security: Applying security best practices, such as input validation, parameterized queries, and implementing security headers, can help mitigate common vulnerabilities and protect against security threats


## Features

- User authentication using jwt
- Wallet Management
- Money Transfer
- Responsive design
- built totally using MongoDB, Express.js, React.js, Node.js


