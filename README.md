# atlasdemo
Atlas CRUD

#### Env File
.env 파일 생성

````
MONGODB=mongodb+srv://USER_ID:PASSWORD@cluster1.5qjlg.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
DATABASE=DATABASENAME
````

#### NPM Install

`````
$ npm install
$ npm install -D nodemon
`````

#### NPM start

`````
$ npm start
`````

#### GET
````
curl --location --request GET 'http://localhost:3000/handson' \
--header 'Content-Type: application/json'
````

#### POST
`````
curl --location --request POST 'http://localhost:3000/handson' \
--header 'Content-Type: application/json' \
--data-raw '{
        "ssn": "123-001-0000",
        "address": {
            "street": "Seoul Jongro-gu, Sejon-ru ",
            "city": "Seoul",
            "zip": 123142
        },
        "name": {
            "firstName":"Jon",
            "lastName" : "Doe"
        },
        "phone": "010-2345-9999"
    }'
`````




