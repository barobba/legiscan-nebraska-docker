INSTALLATION STEPS

1. Start the database server

    docker-compose up -d

2. Then import the database (to the default schema)

    # Go to localhost:8080
    # Make sure to pick "PostgreSQL" in the dropdown
    # Username: postgres
    # Password: password
    # Use the file: ./source/schema-pgsql.sql

3. Build the docker file

    ./dockerfile-build.sh

4. Configure the environment

    cp .env.example .env
    # Add the respecitve values to .env

USAGE

./php.sh legiscan-bulk.php --bulk --import --yes

SEE ALSO

https://api.legiscan.com/dl/
