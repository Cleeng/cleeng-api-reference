autologin()
===========

### Usage

    CleengApi.autologin(callback);

Helper function that can be used to improve experiece for returning customers. If user is logged in to Cleeng platform,
but he doesn't have access token, this method can be used to obtain it automatically.
When call is successful (ie. user is logged to Cleeng Platform), cookie with token will be set.


### Example

    ```javascript
    CleengApi.autologin(function(result) {

        if (result.success) {
            alert("Success! Obtained token: " + result.token);
        }

    });
    ```

[Back to UX API](Reference/UX_API)