purchase()
==========

### Usage

    CleengApi.purchase(itemOfferId, callback);

Opens popup window prompting customer to purchase offer with given ID. If user is not logged in at cleeng.com,
he will be prompted to do so.

#### Params

* **itemOfferId** identifier of item you want to sell
* **callback** function called after popup window is closed (see example below)

#### Example

    CleengApi.purchase(123123123, function(result) {
        if (result.accessGranted) {
            alert('Thank you for buying this item!');
        }
    });

[Back to UX API](Reference/UX_API)