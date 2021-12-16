# atlasdemo
Atlas CRUD

#### Env File
.env 파일 생성

MongoDB 접근 정보 및 사용할 Database 지정    
````
MONGODB=mongodb://USER_ID:PASSWORD@cluster1.5qjlg.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
DATABASE=DATABASENAME
````

#### Local Node test 

`````
$ npm install
$ npm install -D nodemon
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

#### Docker Build
`````
$ docker build -t nodeserver:3.3 .  
$ docker tag nodeserver:3.3  gcr.io/kyudong-kim/nodeserver:3.3 
$ docker push gcr.io/kyudong-kim/nodeserver:3.3 
`````

