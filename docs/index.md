# Welcome to ProApi Documentation

Supercharge your API's with [ProApi](https://proapi.co) 

## Boxes

Boxes in ProApi are simply projects. Each box contains a group of API's which can be used for a particular project which you are working on hence to make it easy to manage project oriented API's.
Each box is identified with their own identification name that is Box ID and it is unique to every box created for each user.
Hence each box can be identified like the one below:
```
https://proapi.co/api/[uname]/[bid]
```
> **uname** : username of your account which you have chosen when creating
>> **bid** : Box ID which is unique to every box created to a particular account

## API's

Each Box can have API's created and similarily each API can be identified by their unique API ID. API can be of type *POST* or *GET*.
```
https://proapi.co/api/[uname]/[bid]/[aid]
```
> **uname** : username of your account which you have chosen when creating
>> **bid** : Box ID which is unique to every box created to a particular account
>>> **aid** : API ID which is unique to every API created.

## How to handle requests

Each API created contains ApiKey which is used to successfully send a request through our secure gateway. Hence when sending request it should be of the following format.
```
POST Request : https://proapi.co/api/[uname]/[bid]/[aid]
```
> **Header** : Header of POST Request should contain apiKey which is unique to each API.
```
apikey: 'APIKEY'
```
> **Body** : The data which you wish to be send through our gateway inside data.
```
data1: 'data1',
data2: 'data2'
```

## Whitelisting

In cases where you want to whitelist the domain from which the API's are being send, then you can use the one below.
```
proapi.co
```