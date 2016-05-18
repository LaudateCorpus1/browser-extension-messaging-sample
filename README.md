Browser extensions messaging sample
===================================

Message exchange between a browser extension content script and background script.
Shows how the messages and responses arrive back in case a document consists of multiple frames or iframes.

Features
--------

* request from a content script with a response via a callback
* message listener on an event coming from a background script

Code
----

* background script (browser-specific): by.js
* content script (browser-specific and shared): log.js, message.js, content.js
* build: gulpfile.js
* test pages (single page, frame and iframe combination): html/*

Setup
-----

* `npm install`
* cd <your favorite browser subdirectory>
* gulp
* build results reside in the 'build' directory

It's possible to generate packages if you place your private keys as

* keys/chrome.pem     (can be generated by Chrome)
* keys/apple-root.pem (see https://github.com/avast/safariextz)
* keys/apple-dev.pem
* keys/dev.pem
* keys/safari.pem


Test
----

Open a page in the 'html' directory
