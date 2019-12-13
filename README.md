# guacamole-docker

This compose stack makes these containers:

- guacamole - the web front end
- guacd - the connection broker
- postgres - the database for auth
- adminer - databse admin

## Running it

1. Run the stack with `docker-compose up -d`
2. Go to http://localhost:8081
3. Log in to the `guacamole-docker_postgres_1` host with `postgres/password`
3. Create a database called `guacamole`
4. Import `initdb.sql` into the `guacamole` database
5. Log in to `http://localhost:8080` with `guacadmin:guacadmin`
6. Change the password and/or create a new user
7. Eat cake

Replace `localhost` with the docker server IP if you're running it somewhere else.

## Support

Not much for me to offer, you're better off looking at guacamole's docs, but feel free to tweet me @TerminalOutcome if you think I can help.