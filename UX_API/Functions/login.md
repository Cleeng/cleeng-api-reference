login()
=======

### Usage

    CleengApi.login(callback);

Opens popup window prompting customer to login to Cleeng platform.

### Example

    CleengApi.login(function(result) {
        if (result.success) {
            alert('You successfuly logged in to Cleeng Platform. Your access token is ' + result.token);
        }
    });

[Back to UX API](Reference/UX_API)