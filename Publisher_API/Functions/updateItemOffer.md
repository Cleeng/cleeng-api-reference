updateItemOffer()
=================

Modifies properties of existing item offer.

#### JSON-RPC example

Example that changes description and price.

Request:

    ```javascript
    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"createItemOffer",
        "params":{
            "token":"wYk4VM7JpHIMaHaFMTynO59PKv90xEL9Rz6X4xCbcbsnukQ-",
            "itemOfferId":707221016,
            "itemOfferData":{
                "description":"This is updated description",
                "price":1.99,
            }
        },
    }
    ```

Response:

When call is successful, all item offer properties are returned.

    ```javascript
    {
        "jsonrpc":"2.0",
        "id":"1",
        "error":null,
        "result":{
            "id":123123123,
            "url":"http://your-site.com/view-item-here",
            "type":"article",
            "pageTitle":"My Blog",
            "price":1.99,
            "publisherId":"123123123",
            "currency":"USD",
            "currencySymbol":"\u00a3",
            "description":"This is updated description",
            "socialCommissionEnabled":false,
            "socialCommissionRate":null,
            "shortUrl":"http://cleeng.it/m0zdx7",
            "hasLayerDates":false,
            "layerStartDate":null,
            "layerEndDate":null,
            "publisherName":"John McBlogger",
            "averageRating":4,
            "createdAt":"2011-12-24 18:54",
            "updatedAt":"2011-12-24 18:54",
            "myId":"",
            "myData": ""
        }
    }
    ```

[Back to Publisher API](Reference/Publisher_API)