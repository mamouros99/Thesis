To build the project:
docker compose build
docker compose up

To build the project locally: Change .env profile to dev

To run locally:
Run desktop & mobile: VUE_APP_ENV_FILE=dev quasar dev

Run backend: ./gradlew bootrun