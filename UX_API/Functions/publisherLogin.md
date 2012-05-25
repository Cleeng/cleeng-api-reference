publisherLogin()
================

### Usage

    CleengApi.publisherLogin(appSecureKey, callback);

Opens popup window prompting publisher to login to Cleeng platform. After completing this process user will
receive access token that will give him rights to call Publisher API functions.
If user is does not have publisher account yet, he will be prompted to fill in "account upgrade form".

Sometimes you may need to allow multiple publishers to login to Cleeng from single backend, to allow them
publishing items on their behalf. This function will allow publishers to do so, triggering login screen.
After filling credential information, publisher will have to confirm (by clicking on a button), that he wants
to connect to your backend.

To be able to use this function, you need to provide Cleeng Javascript SDK with two values: "application ID"
and "application secret". They can be obtained from [here](https://cleeng.com/dev/api-keys) (this page will
be accessible after logging in to your main publisher account).

Before calling publisherLogin(), you need to supply Application Id to `CleengApi.setAppId()` function (see
example below).

### Example

    CleengApi.setAppId('ZX0WOj8b0qthW3w5Cc9tHAoBvD928ctDNZElFlGXd640CDUA');
    CleengApi.publisherLogIn('cbsn-wYk4VM7JpHIMaHaFMukQYmFEY2de090xEL9Rz6X4xCb', function(result) {
        if (result.success) {
            alert('You are now allowed to use publisher API. Your access token is ' + result.token + ' - keep it safe!');
        }
    });

[Back to UX API](Reference/UX_API)