Symfony3ApiRest
========================

[![Build Status](https://travis-ci.org/Tony133/Symfony3ApiRest.svg?branch=master)](https://travis-ci.org/Tony133/Symfony3ApiRest)

Simple Api Rest with Symfony 3

## Install with Composer

```
    $ curl -s http://getcomposer.org/installer | php
    $ php composer.phar install or composer install
```

## Getting with Curl

```
    $ curl -H 'content-type: application/json' -v -X GET http://127.0.0.1:8000/api/users
    $ curl -H 'content-type: application/json' -v -X GET http://127.0.0.1:8000/api/users/:id
    $ curl -H 'content-type: application/json' -v -X POST -d '{"name":"test","surname":"test"}' http://127.0.0.1:8000/api/users
    $ curl -H 'content-type: application/json' -v -X PUT -d '{"name":"test","surname":"test"}' http://127.0.0.1:8000/api/users/:id
    $ curl -H 'content-type: application/json' -v -X DELETE http://127.0.0.1:8000/api/users/:id
```

## Pagination with Curl

```
    $ curl -H 'content-type: application/json' -v -X GET http://127.0.0.1:8000/api/users?page=:number_page 
```

## User Authentication with Curl

```
    $ curl -H 'content-type: application/json' -v -X GET http://127.0.0.1:8000/api/users  -H 'Authorization:Basic username:password'
```
