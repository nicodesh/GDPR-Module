# Cookie Level Consent Manager

This module makes your life easier to be GDPR compliant about the Cookie Privacy Policy.

This webusers will be able to choice between three consent levels : technical cookies, analytics cookies, marketing cookies.

## Getting Started

You just have a index.html, which is an (almost) empty exemple of a web page.

Inside, you can find the HTML bloc, compound of 3 div tags.

Then, you have a CSS file that you have to call on each web page.

And finally, the JavaScript code that you have to call before the closing body tag.

### Prerequisites

This module was made to run with GTM, but you can easily rearange it if you want to make it run with another TMS or even without TMS.

### Installing

1. Include the HTML part in all your web pages.
2. Call the CSS file in all your web pages.
3. Call the JS file in all your web pages, in the footer, juste before the body closing.

That's it!

## Settings

There are three consent levels.

1. Technical cookies only.
2. Technical cookies + Analytics cookies
3. Technical cookies + Analytics cookies + Marketing cookies

The module is in french, so you have to adapt the text content of :

1. The main text in the pop-in
2. Each text of each consent level
3. The band content

All pop-in text contents are push in JavaScript, in order to be SEO friendly.

You can check the JavaScript file to change the name of the cookie.

## Testings

If everything is okay, a cookie is set with one of those three different values:

'level1' or 'level2' or 'level3'.

And then, the module will send one or several "dataLayer.push({})" for each page loading.

Cookie value: 'level1'
Actions:
dataLayer.push({'event': 'level1'});

Cookie value: 'level2'
Actions:
dataLayer.push({'event': 'level1'});
dataLayer.push({'event': 'level2'});

Cookie value: 'level3'
Actions:
dataLayer.push({'event': 'level1'});
dataLayer.push({'event': 'level2'});
dataLayer.push({'event': 'level3'});

## Author

* **Nicolas Deschamps de Boishebert**

## Acknowledgments

* Thanks to the Digimood Team :)