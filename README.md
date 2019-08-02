# coa_flask_app

[![Build Status](https://travis-ci.com/CleanOceanAction/coa_flask_app.svg?branch=master)](https://travis-ci.com/CleanOceanAction/coa_flask_app)

The flask back-end REST APIs for the COA website.

## Getting Started

1. Install python3.7 and pipenv or have docker installed.
    - `sudo apt install python3.7`
    - `sudo python3.7 -m pip install pipenv`
    - or
    - `sudo apt install docker`
2. Setup DB related environment variables (not posted here for security reasons).
3. Start the server
    - `make run`

## Testing

To test that the flask app is running and properly connected to the database,
use the curl command.

- `curl localhost:5000/locations`

Or to hit the deployed instance.

- `curl http://coa-flask-app-prod.us-east-1.elasticbeanstalk.com/locations`

## Inspecting the Database

1. Install MySQL Workbench [here](https://dev.mysql.com/downloads/workbench/)
2. In MySQL Workbench click on 'MySQL Connections +' to add
   a connection with AWS RDS.
3. Enter the hostname, port, username, and password using the
   same credentials mentioned in the `CONTRIBUTING.md`.
4. From the 'Home' view, you can click on the connection to inspect the database.