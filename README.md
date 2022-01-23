
# Inavitas NodeJS Bootcamp Graduate Project Group 2

## School Energy Tracking System

With this project, we will be able to monitor the temperature, air quality and average electricity consumption of the classrooms. 3 different sensors will be generate and simulated data in seconds. This data will be retrieved from PostgreSql and Redis with Reader API. This data will first be added to the queue by the Manufacturer. The consumer will receive this data and save it in databases. It also logs all errors to MongoDB with another API.

![App Screenshot](https://raw.githubusercontent.com/P149-Bootcamp-Graduation-Project/Group3/main/img/proje_2022-01-05_14-40-33.png)





## Installation
Clone First
```bash
 git clone https://github.com/P149-Bootcamp-Graduation-Project/Group3
```

To run each API

```bash
  npm i
  node app.js
```

## Authors

- [@İlyas Yağcıoğlu](https://github.com/ilyas9461)
- [@Oğuzhan Eyerci](https://github.com/oguzeyerci)
- [@Atakan Dönmez](https://github.com/atakandnmz)

## Acknowledgements

 - [Kafka-Node](https://www.npmjs.com/package/kafka-node)
 - [Redis](https://redis.io/documentation)
 - [MongoDb](https://docs.mongodb.com/drivers/node/current/)
 - [PostgreSql](https://node-postgres.com/)
 - [Swagger](https://www.npmjs.com/package/express-swagger-generator)
 - [Sercan Reyhanlı](https://github.com/IvanBarayev)



## Tech Stack

**Server:** Node, Express   
**Databases:** PostgreSql (for main database), MongoDb (for error logs), Redis (for cache)  
**Other:** Docker, Kafka (for queue), Swagger (for Documentation)


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

    PGHOST=88.198.26.82
    PGPORT=5432
    PGUSER=group2
    PGPASSWORD=Password1
    PGDATABASE=patika

    REDIS_HOST=88.198.26.82
    REDIS_PORT=6379
    REDIS_INDEX=2
    REDIS_PASS=dd3j5sKmUHVD6xpG

    MONGODBNAME = test
    MONGOURI = mongodb+srv://ivanbarayev:tDVRDyxJbdjF7k9G@docdb.xmg8e.mongodb.net/?ssl=true&authSource=admin

    producer-temp-api APP_PORT=9461
    producer-power-api APP_PORT=9462
    producer-air-api APP_PORT=9463

    consumer-temp-api APP_PORT=9464
    consumer-power-api APP_PORT=9465
    consumer-air-api APP_PORT=9466

    error-logger-api APP_PORT=9467

    APP_HOST=127.0.0.1                      
    