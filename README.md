
# How to Run Project

## Locally

> Required: 
> - Mysql DB;
> - In fenix.tecnico create two distinct apps.  The urls will depend upon the chosen ports for the frontend web apps.



#### Frontend: desktop-app

Create .env.local from .env.example

Run:
```
 VUE_APP_ENV_FILE=local quasar dev 
```

#### Frontend: mobile-app
Create .env.local from .env.example

Run:
```
 VUE_APP_ENV_FILE=local quasar dev 
```

#### Backend 

Create *application.properties* based on *application-example.properties*:
1.  DataBase section with approriate **username**, **password** and **url** (MYSQL)
2.   **desktop** & **mobile url's** to appropriate ports
3.  **server.port** to desired port
4.  Desktop section and Mobile section with the parameters from the previously defined apps (fenix)
5. Email section with proper

Run ./gradlew bootRun

---

## Docker Locally

#### Backend
On the backend folder:
Update application-dev.properties

./gradlew clean build -x test

#### Frontend: mobile-app
Update .env.dev


#### Frontend: mobile-app
Update .env.dev


#### Docker:
Change  .env on thesis folder. profile=dev
On the thesis page:
```
docker compose down;
docker compose build;
docker compose up -d;
```

---

## Docker Server

#### Backend
On the backend folder:
Update application-prod.properties

./gradlew clean build -x test

#### Frontend: mobile-app
Update .env.prod


#### Frontend: mobile-app
Update .env.prod


#### Docker:
Change  .env on thesis folder. profile=prod
On the thesis page:
```
docker compose down;
docker compose build;
docker compose up -d;
```

---
