Third party cookie check for browsers
=====================================

A simple, static, passive (CDN-compatible) way of checking if third party cookies are enabled in a browser.
Consists of two scripts - one that will set a cookie (start.html), and another that will post a message depending on if the
cookie is present or not (complete.html).

Deploy the two scripts somewhere on a different domain from the main application, then load them using check.html.

## Live example

Thanks to github pages, the scripts are hosted already at https://learningscience.github.io/3rdpartycookiecheck/start.html -- so you can use that as a live version. For production, it's better to deploy somewhere under your control.

To see the client code in action, run this JSFiddle: https://jsfiddle.net/tugawg8y/

## Changes from fork
* Cookie renamed
* Message renamed
* Moved example code into check.html
* Added timeout that sets third part cookies as unsupported after 10 seconds if no message is received from complete.html
