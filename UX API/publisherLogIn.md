publisherLogin
==============

Usage:
    CleengApi.publisherLogin(appSecureKey, callback);

Opens popup window prompting publisher to login to Cleeng platform. After completing this process user will
receive access token that will give him rights to call Publisher API functions.
If user is does not have publisher account yet, he will be prompted to fill in "account upgrade form".

### Example:

    CleengApi.publisherLogIn('cbsn-wYk4VM7JpHIMaHaFMukQYmFEY2de090xEL9Rz6X4xCb', function(result) {
        if (result.success) {
            alert('You are now allowed to use publisher API. Your access token is ' + result.token + ' - keep it safe!');
        }
    });
