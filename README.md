# HashiCorp.com

This is the repository for the [main HashiCorp website](http://www.hashicorp.com).

This is a [Middleman](http://middlemanapp.com) project, which builds a static
site from these source files. The site is hosted on [Heroku](http://heroku.com)
and then fronted by [Fastly](http://fastly.com).

## Contributions Welcome!

If you find a typo or you feel like you can improve the HTML, CSS, or
JavaScript, we welcome contributions. Feel free to open issues or pull
requests like any normal GitHub project, and we'll merge it in.

## Running the Site Locally

Running the site locally is simple. Clone this repo and run the following
commands:

```
$ bundle
$ bundle exec middleman server
```

Then open up `localhost:4567`. Note that some URLs you may need to append
".html" to make them work (in the navigation and such).

## Stylesheets

We use [Less](http://lesscss.org) to generate site-specific stylesheets along
with [Bootstrap](http://getbootstrap.com). [Grunt](http://gruntjs.com)
is used to create a watcher for changes to the `.less` files.  The
watcher re-compiles the hashicorp.css file when it detects changes in
the .less files.

Assuming you have [npm](http://npmjs.com), 
[node.js](http://node.js), and [Less](http://lesscss.org) installed, you can install and run Grunt
and the watcher this way:

```
$ npm install -g grunt-cli
$ npm install
$ grunt
```
