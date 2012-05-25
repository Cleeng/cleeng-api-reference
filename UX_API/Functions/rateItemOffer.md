rateItemOffer()
===============

### Usage

    ```javascript
    CleengApi.rateItemOffer(itemOfferId, liked, callback);
    ```

Helper function for improving user's experience. It allows customers to say if they liked
given item or not. Rating will be shown in their library. It is also available from
[getItemOffer()](Reference/Query_API/Functions/getItemOffer) API (`averageRating` property).

Rating can be done only once, by users who purchased given item.


### Example

    ```javascript
    // when user clicks on thumbs up icon, we should notify Cleeng Platform
    $('#thumbs-up').click(function() {
        CleengApi.rateItemOffer(123123123, true);
    });
    ```

[Back to UX API](Reference/UX_API)