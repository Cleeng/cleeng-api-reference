getSubscriptionStatus()
=======================

Usage:
  getSubscriptionStatus(token, publisherId)


similar to getAccessStatus, but will


Request:

    ```javascript
    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"getAccessStatus",
        "params":{
            "token":"cZhBnXbXgacAwImgxoV6gnj7-kiDhb6G17qyYfV-bmxlFGSA",
            "publisherId":123123123
        }
    }
    ```

Response:

    ```javascript
    {
        "jsonrpc":"2.0",
        "id":"1",
        "error":null,
        "result":{
            "subscribed":true,
            "subscriptionType":"monthly",
            "subscriptionStatus":"paused",
            "expirationDate":"2011-12-24 18:54"
        }
    }
    ```

[Back to Query API](Reference/Query_API)