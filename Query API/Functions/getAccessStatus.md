getAccessStatus()
=================

Usage:
    getAccessStatus(token, itemOfferId)

#### JSON-RPC example

Request:

    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"getAccessStatus",
        "params":{
            "token":"cZhBnXbXgacAwImgxoV6gnj7-kiDhb6G17qyYfV-bmxlFGSA",
            "itemOfferId":123123123
        }
    }

Response:

    {
        "jsonrpc":"2.0",
        "id":"1",
        "error":null,
        "result":{
            "accessGranted":true,
            "voted":false,
            "socialCommissionUrl":"http://cleeng.it/kXpd2Q"
        }
    }


[Back to Query API](wiki/Reference/Query%20API)