#### Setup

```bash
npm install && npm start
```

#### Database Connection

1. Import connect.js
2. Invoke in start()
3. Setup .env in the root
4. Add MONGO_URI with correct value

#### Query examples

- /products?name=wooden
- /products?company=ikea
- /products?featured=true
- /products?sort=-name,price
- /products?fields=company,rating

#### Routers

- products.js

#### Product Model

Company Validation

```
enum: {
      values: ["ikea", "liddy", "caressa", "marcos"],
      message: "{VALUE} is not supported",
    },
```

#### Product query

Sort products according to their:

- name
- price
- rating
- company
- creation date
