createItemOffer()
=================

#### JSON-RPC example

Request:

    {
        "jsonrpc":"2.0",
        "id":1,
        "method":"createItemOffer",
        "params":{
            "token":"wYk4VM7JpHIMaHaFMTynO59PKv90xEL9Rz6X4xCbcbsnukQ-",
            "itemOfferData":{
                "url":"http://your-site.com/view-item-here",
                "description":"Buy this item for just $0.49. You will love it!",
                "pageTitle":"My Blog",
                "price":0.99,
                "type":"article"
            }
        },
    }

Response:

    {
        "jsonrpc":"2.0",
        "id":"1",
        "error":null,
        "result":{
            "id":123123123,
            "url":"http://your-site.com/view-item-here",
            "type":"article",
            "pageTitle":"My Blog",
            "price":0.99,
            "publisherId":"123123123",
            "currency":"USD",
            "currencySymbol":"\u00a3",
            "description":"Buy this item for just $0.49. You will love it!",
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



- add info about "read-only" properties

[Back to Publisher API](Reference/Publisher_API)