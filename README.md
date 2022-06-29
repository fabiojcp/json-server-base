# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth.

## Base

https://server-test-fabiojcp.herokuapp.com

## Endpoints

# Register 

/register

method: POST

JSON:
{
    email: "email"
    password: "password"
}

Return:

200 CREATED

{
	"accessToken": "token",
	"user": {
		"email": "email",
		"id": "userID
	}
}

# Login

/login

method: POST

JSON:

{
    name: "name"
    password: "password"
}

Return:

200 OK

{
	"accessToken": "token",
	"user": {
		"email": "email",
		"id": "userID"
	}
}

# User

/600/users/:userID

method: GET

Header:

Authorization: Bearer "token"

Return:
200 ok

{
	"email": "email",
	"password": "crypto password,
	"id": "userID"
}