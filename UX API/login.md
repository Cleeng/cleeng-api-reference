login
=====

usage: 
    login(callback);

Opens popup window prompting customer to login to Cleeng platform.

    CleengApi.login(function(result) {
        if (result.success) {
            alert('You successfuly logged in to Cleeng Platform. Your access token is ' + result.token);
        }
    });