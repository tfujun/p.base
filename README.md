# p.base
base python setup with docker containerization following https://youtu.be/6OxqiEeCvMI?si=Kt83pgg457N7H7jo

# How to use
1. update `Docker-compose.yml` with container name.
2. If needed, update the `volumes` config to change the name of the folder inside the container to bind to
3. Add more apps as needed to run different applications inside the same container that the main python app may be dependent on (eg. redis, dynamodb, etc.)
4. run the following command to spin up the container:
```
docker compose up --build -d
```
5. When done run `docker compose down`