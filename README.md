# Ecommerce website
## About the website
This is ecommerce websitw which is selll the coffee capsules
## Files includes
HTML and CSS 
* vertuo.html
* main.css
* image floder

Server side JavaScript 
* server.js
* server.test.js

Client side Javascript
* main.js

Others
* coffee.json
* cart.json
* .eslintrc.js
* package.json
* package-lock.json

## How execute the code 
### In the terminal/shell
```
npm install
```
```
npm start
```
```
http://127.0.0.1:8081/vertuo.html
```
## Run the test
### Eslint
```
npm run pretest
```
### Jest test
```
npm test
```


### REST API
```
https://documenter.getpostman.com/view/26074133/2s93CUH9oP
```

## Get list of Things

### Request

`GET /coffee/`

    curl --location 'http://127.0.0.1:8081/coffee'

### Response


    {
    "vertuo": [
        {
            "name": "altissio decaffeinato",
            "id": "1",
            "intensity": "9",
            "type": "espresso",
            "price": "0.50",
            "image": "image/altissio-decaffeinato.jpeg"
        },
        {
            "name": "altissio",
            "id": "2",
            "intensity": "9",
            "type": "espresso",
            "price": "0.48",
            "image": "image/altissio.jpeg"
        },
        {
            "name": "arondio",
            "id": "3",
            "intensity": "6",
            "type": "Gran Lungo",
            "price": "0.56",
            "image": "image/arondio.jpeg"
        },
        {
            "name": "bianco doppio",
            "id": "4",
            "intensity": "N/A",
            "type": "doble espresso",
            "price": "0.56",
            "image": "image/bianco-doppio.jpeg"
        },
        {
            "name": "bianco piccolo",
            "id": "5",
            "intensity": "N/A",
            "type": "espresso",
            "price": "0.53",
            "image": "image/bianco-piccolo.jpeg"
        },
        {
            "name": "biancoforte",
            "id": "6",
            "intensity": "N/A",
            "type": "Mug",
            "price": "0.65",
            "image": "image/biancoforte.jpeg"
        },
        {
            "name": "caramel cookie",
            "id": "7",
            "intensity": "N/A",
            "type": "Mug",
            "price": "0.65",
            "image": "image/caramel-cookie.jpeg"
        },
        {
            "name": "chocolate fudge",
            "id": "8",
            "intensity": "N/A",
            "type": "Mug",
            "price": "0.65",
            "image": "image/chocolate-fudge.jpeg"
        },
        {
            "name": "colombia",
            "id": "9",
            "intensity": "5",
            "type": "Mug",
            "price": "0.69",
            "image": "image/colombia.jpeg"
        },
        {
            "name": "costarica",
            "id": "10",
            "intensity": "7",
            "type": "Gran Lungo",
            "price": "0.62",
            "image": "image/costarica.jpeg"
        },
        {
            "name": "diavolitto",
            "id": "11",
            "intensity": "11",
            "type": "espresso",
            "price": "0.48",
            "image": "image/diavolitto.jpeg"
        },
        {
            "name": "double espresso chiaro",
            "id": "12",
            "intensity": "8",
            "type": "double espresso",
            "price": "0.55",
            "image": "image/double-espresso-chiaro.jpeg"
        },
        {
            "name": "double espresso dolce",
            "id": "13",
            "intensity": "5",
            "type": "double espresso",
            "price": "0.55",
            "image": "image/double-espresso-dolce.jpeg"
        },
        {
            "name": "Ethiopia",
            "id": "14",
            "intensity": "4",
            "type": "Gran Lungo",
            "price": "0.62",
            "image": "image/ethiopia.jpeg"
        },
        {
            "name": "fortado decaffeinato",
            "id": "15",
            "intensity": "8",
            "type": "Gran Lungo",
            "price": "0.58",
            "image": "image/fortado-decaffeinato.jpeg"
        },
        {
            "name": "fortado",
            "id": "16",
            "intensity": "8",
            "type": "Gran Lungo",
            "price": "0.56",
            "image": "image/fortado.jpeg"
        },
        {
            "name": "Half caffeinato",
            "id": "17",
            "intensity": "5",
            "type": "Mug",
            "price": "0.64",
            "image": "image/half-caffeinato.jpeg"
        },
        {
            "name": "Hezelio muffin",
            "id": "18",
            "intensity": "N/A",
            "type": "Mug",
            "price": "0.65",
            "image": "image/hezelio-muffin.jpeg"
        },
        {
            "name": "II caffe",
            "id": "19",
            "intensity": "11",
            "type": "espresso",
            "price": "0.48",
            "image": "image/il-caffe.jpeg"
        },
        {
            "name": "Inizio",
            "id": "20",
            "intensity": "4",
            "type": "Gran Lungo",
            "price": "0.56",
            "image": "image/inizio.jpeg"
        },
        {
            "name": "Intenso",
            "id": "21",
            "intensity": "9",
            "type": "Mug",
            "price": "0.62",
            "image": "image/intenso.jpeg"
        },
        {
            "name": "Melozio decaffeinato",
            "id": "22",
            "intensity": "6",
            "type": "Mug",
            "price": "0.64",
            "image": "image/melozio-decaffeinato.jpeg"
        },
        {
            "name": "Melozio",
            "id": "23",
            "intensity": "6",
            "type": "Mug",
            "price": "0.62",
            "image": "image/melozio.jpeg"
        },
        {
            "name": "Mexico",
            "id": "24",
            "intensity": "7",
            "type": "Mug",
            "price": "0.69",
            "image": "image/mexico.jpeg"
        }
    ]}


## Create a new Thing

### Request

`POST /checkout/`

 ```
 curl --location 'http://127.0.0.1:8081/checkout' \
--data '
{"name": "altissio decaffeinato",
"price": "0.50",
"quantity": 2}'
 ```


### Response

    [
    {
        "name": "altissio decaffeinato",
        "id": "1",
        "intensity": "9",
        "type": "espresso",
        "price": "0.50",
        "image": "image/altissio-decaffeinato.jpeg",
        "quantity": 2
    }]


## Get a specific Thing


### Request

`GET /cart/`

    curl --location 'http://127.0.0.1:8081/cart'

### Response

  ``` [
    {
        "name": "altissio decaffeinato",
        "id": "1",
        "intensity": "9",
        "type": "espresso",
        "price": "0.50",
        "image": "image/altissio-decaffeinato.jpeg",
        "quantity": 1
    },
    {
        "name": "altissio",
        "id": "2",
        "intensity": "9",
        "type": "espresso",
        "price": "0.48",
        "image": "image/altissio.jpeg",
        "quantity": 1
    }
]
```

