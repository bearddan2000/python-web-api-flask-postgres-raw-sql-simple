# python-web-api-flask-postgres-raw-sql-simple

## Description
Creates an api of `dog` by using raw sql for a flask project.
Has the ability to query by parameters.
If path is not found, will default to 404 error.

Remotely tested with *testify*.

## Tech stack
- python
  - flask
  - sqlalchemy
  - testify
  - requests

## Docker stack
- python:latest
- postgres

## To run
`sudo ./install.sh -u`
- Get all dogs: http://localhost/dog
  - Schema id, breed, and color
- CRUD opperations
  - Create: curl -i -X PUT localhost/dog/<id>
  - Read: http://localhost/dog/<id>
  - Update: curl -i -X POST localhost/dog/<id>/<breed>/<color>
  - Delete: curl -i -X DELETE localhost/dog/<id>

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`
