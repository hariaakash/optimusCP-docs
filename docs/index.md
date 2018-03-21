# Getting Started

Manage - Collaborate - Automate - Monitor with [OptimusCP](https://optimuscp.io)

## API Key Generation

From Dashboard head over to the API section from left sidebar and generate a API Key which will be used for authentication of the request.
> **APIKEY** should be kept confidential otherwise any one with APIKEY can access your server.

## Types of Request

Requests can be either *POST* or *GET*. For detailed information refer [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods).

## Division

OptimusCP has a Profile/Personal Dashboard and separate Dashboard for teams. Hence the APIKEY & API endpoint for your personal server varies with the one belonging to your team.


# Personal Servers

## Servers List

To get the list of servers which are available in your Personal Dashboard.
> **Request** : The HTTP method to be used for the below endpoint.
```
GET
```
> **Header** : API Endpoint.
```
https://optimuscp.io/api/servers
```
> **Header** : Header of Request.
```
apikey: "APIKEY"
```

## Server Information

To get information about one particular server.
> **Request** : The HTTP method to be used for the below endpoint.
```
GET
```
> **Header** : API Endpoint.
```
https://optimuscp.io/api/server
```
> **Header** : Header of Request.
```
apikey: "APIKEY"
```
> **PARAMS** : Parameters of Request.
```
serverId: "Server Unique ID"
```

## Server Execution
To execute a particular command on your server.
> **Request** : The HTTP method to be used for the below endpoint.
```
POST
```
> **Header** : API Endpoint.
```
https://optimuscp.io/api/server/exec
```
> **Header** : Header of Request.
```
apikey: "APIKEY"
```
> **BODY** : Body of Request.
```
serverId: "Server Unique ID",
cmd: "1st command ;2nd command & 3rd command"
```
