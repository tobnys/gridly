
[![gridly](http://i.imgur.com/kPrOESX.png)](http://ionicabizau.github.io/gridly/example/)

# gridly

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Version](https://img.shields.io/npm/v/gridly.svg)](https://www.npmjs.com/package/gridly) [![Downloads](https://img.shields.io/npm/dt/gridly.svg)](https://www.npmjs.com/package/gridly)

> The minimal (~100-170 bytes) grid system for modern browsers.


You don't need monolithic CSS frameworks for simple grid systems. ~100 bytes of CSS can save your life. :dizzy:

## Usage

In the [`dist`](/dist) directory there are three minified files:


 - `gridly-core.min.css` (105 B): just the Gridly core including same-width column support and mobile responsive support.
 - `gridly-col-widths.min.css` (115 B): the custom width columns
 - `gridly.min.css` (165 B): the previous two files' content put together


If you need to support more browsers, you can use the prefixed versions. They're located in [`dist/prefixed`](/dist/prefixed). They're ~1.8× the size of their counterparts.

### Browser Support

Gridly supports browsers that implement the Flexible Box Layout Module.

As of December 2015, [browser support for flexbox](http://caniuse.com/#feat=flexbox) is 81.27% for unprefixed, and 95.44% for prefixed.

## :rocket: Available on CDN!

Gridly is available on cdnjs.com. [**Check it out**](https://cdnjs.com/libraries/gridly).

> https://cdnjs.cloudflare.com/ajax/libs/gridly/1.1.0/gridly-core.min.css
> https://cdnjs.cloudflare.com/ajax/libs/gridly/1.1.0/gridly-col-widths.min.css
> https://cdnjs.cloudflare.com/ajax/libs/gridly/1.1.0/gridly.min.css


If you do not need custom width columns, you will probably want to use only `gridly-core.min.css` in your page. If you do need the custom width columns, you have to include `gridly.min.css` instead.

## Example

Include the CSS file in your page:

```html
<link rel="stylesheet" href="gridly.min.css" type="text/css" charset="utf-8">
```

Then you can use the `.row` and `.col` classes:

```html
<div class="row">
    <div class="col">Two</div>
    <div class="col">Column</div>
</div>
```

This will create two columns having equal widths.


[![gridly](http://i.imgur.com/m4pwrnO.png)](http://ionicabizau.github.io/gridly/example/)

## :cloud: Installation


Check out the [`dist`](/dist) directory to download the needed files and include them on your page.

If you're using this module in a CommonJS environment, you can install it from `npm` and `require` it:

```sh
$ npm i --save gridly
```


## :memo: Documentation


The `gridly-core.min.css` file handles two classes:


 - `row`: the row containing columns
 - `col`: the column to put in the row


Because of the flexbox amazing power, the columns will have the same width (as many columns you want / row).


To extend this basic functionality, there is another file: `gridly-col-widths.min.css`. This adds the following classes:


 - `col-tenth` has `10%` width
 - `col-fifth` has `20%` width
 - `col-quarter` has `25%` width
 - `col-third` has `33.3333334%` width
 - `col-half` has `50%` width


Like specified above, the `gridly.min.css` contains both: the core and the custom widths.


## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:



Run `npm i` to install the dependencies. Then, you can run the npm scripts using `npm run <script-name>`.


Run `npm run release` to recreate all the `dist` files.


## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:



 - [showalicense.com](http://showalicense.com/)–A site to provide an easy way to show licenses and their human-readable explanations. ([source](https://github.com/IonicaBizau/showalicense.com))


## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
