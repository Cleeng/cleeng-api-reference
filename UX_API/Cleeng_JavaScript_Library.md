Cleeng JavaScript Library
=========================

In order to be able to use Cleeng JavaScript API, you need to include following JS file in your HTML document:

    http://cdn.cleeng.com/js-api/2.0/api.js

API is accessible with CleengApi class. It provides access to two different types of functionality:

* query API (via JSONP)
* UX API

UX API is used to perform tasks that require interaction from customer, like purchasing (where he needs
to type his credit card number, etc). Most of this functionalities will take place in popup window, where user will
be prompted to log in, type payment details, and so on. After finishing given task, popup window will be closed
and you will recevie some information, indicating for example if customer can now access given item.


Due to asynchronouns nature of JavaScript, most API methods can take callback function as its parameter.
This callback will be executed after given task is finished. This means that after calling any of this
APIs, your JavaScript is not blocked and will continue to execute.

To understand above, see following example:

    CleengApi.purchase(123123123, function(result) {
        alert('This alert box will appear after finishing purchase.');
    });
    alert('This alert box will appear together with purchase popup window!');

[Back to UX API](Reference/UX_API)
