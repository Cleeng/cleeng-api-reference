getPublisherSubscriptions()
===========================

Usage:
  getPublisherSubscriptions(publisherId)


Returns list of subscription plans created by given publisher.


Request:

    ```javascript
    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"getPublisherSubscriptions",
        "params":{
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
            "hasSubscriptionOffer":true,
            "subscriptionPrompt":"Subscribe now!",
            "availablePlans":[
                {
                    "type":"weekly",
                    "currency":"EUR",
                    "price":"5.99"
                },
                {
                    "type":"monthly",
                    "currency":"EUR",
                    "price":"15.99"
                }
            ]
        }
    }
    ```

[Back to Query API](Reference/Query_API)