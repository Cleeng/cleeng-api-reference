getUserInfo()
=============


Usage:
    getUserInfo(token)

Returns information about user identified by given token.

#### Params

* **token** access token used to identify user on Cleeng platform

#### Return data

If valid token is passed, getUserInfo() will return JSON object with following
properties:

* **id** user's ID
* **name** user name
* **accountType** "customer" or "publisher"
* **currency** user's currency: USD, EUR, GBP
* **currencySymbol** dollar, euro or pond sign
* **locale** "en_US", "fr_FR", "nl_NL"
* **country** two-letter country symbol
* **publisherAccess** boolean value indicating if user can call publisher's API functions with provided token


#### JSON-RPC example

Request:

    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"getUserInfo",
        "params":{
            "token":"cZhBnXbXgaci17qyYAwImgxoV6gnj7-kfV-bmDhb6GxlFGSA"
        },
    }


Response:

    {
        "jsonrpc":"2.0",
        "id":"1",
        "error":null,
        "result":{
            "id":"702731750",
            "name":"John McBlogger",
            "accountType":"publisher",
            "currency":"USD",
            "currencySymbol":"$",
            "locale":"en_US",
            "country":"US",
            "publisherAccess":false
        }
    }

[Back to Query API](Reference/Query_API)