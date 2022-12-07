<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Run in development
1. Clone the repository
2. Run
```
yarn install
```
3. Have nestjs cli intalled.
```
npm i -g @nest/cli 
```
4. Start the database
```
docker-compose up -d
```
5. Clone file ```.env.template``` and rename ``` .env ```

6. fill environment variables

7. run app with
```
  yarn start:dev
```

6. Rebuild database with see
```
localhost:3000/api/v2/seed
```

## Used Stack 
* Mongo DB
* Nest
* Docker

# Production Build
1. Create file ```.env.prod```
2. Fill Prod environment variables
3. Create new image
```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build -d
``` 