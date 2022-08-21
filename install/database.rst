Database storage
===================================

Data will be stored in plain text if no credentials.json file is configured. You can use the webapp that way without further configuration.

However, you can choose to persist in your data in postgres, mysql, or any relational database supported by `knexjs <https://knexjs.org/>`, the database manager. 

For example, create a credentials.json file with the folowing JSON to store your data in a sqlite database::

    {
        client: 'sqlite3',
        connection: {
            filename: "/app/data/api/mydb.sqlite"
        }
    }


Add the folowing startup parameter : -v ```pwd```/credentials.json:/app/credentials.json
