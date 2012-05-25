getItemOffer()
==============

Usage:
    getItemOffer(itemOfferId)

#### JSON-RPC example

Request:

    ```javascript
    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"getItemOffer",
        "params":{
            "itemOfferId":123123123
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
            "id":"123123123","
            "url":"http://your-site.com/view-item-here",
            "pageTitle":"My Blog",
            "price":"0.0000",
            "publisherId":"328738825",
            "currency":"USD",
            "currencySymbol":"$"
            "description":"Buy this item for just $0.49. You will love it!",
            "socialCommissionEnabled":false,
            "socialCommissionRate":"0.00",
            "shortUrl":"http://cleeng.it/kXpd2Q",
            "type":"article",
            "hasLayerDates":false,
            "layerStartDate":null,
            "layerEndDate":null,
            "myId":"0",
            "publisherName":"John McBlogger",
            "averageRating":4,
        }
    }
    ```


#### JavaScript example

    ```javascript
    CleengApi.getItemOffer(123123123, function(itemOffer) {
        alert('Item description: ' + itemOffer.description);
    });
    ```


[Back to Query API](Reference/Query_API)