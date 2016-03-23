---
layout: documentation
title: Installation
next: application
---

# Installation

You can install T3 on your web page or application in a few different ways.

## Downloading T3 Locally

You can always download the latest version of T3 from our [GitHub repository](https://github.com/box/t3js). The `dist` directory contains the latest files you'll need to use T3:

* `t3.js` - Latest unminified version of T3. Supports IE9+
* `t3.min.js` - Minified version of t3.js
* `t3-jquery.js` - Latest unminified version of T3 - Supports IE8+ with [jQuery](http://jquery.com/)
* `t3-jquery.min.js` - Minified version of t3-jquery.js

For development, we recommend downloading `t3.js` while for production `t3.min.js` is more appropriate to reduce the file size.

## Downloading T3 with npm

You can download T3 using [npm](https://npmjs.com):

{% highlight shell %}
$ npm i t3js --save
{% endhighlight %}

This installs T3 into `node_modules/t3js`. The package includes the `dist` directory from the GitHub repository, so you can include T3 in your page like this:

{% highlight html %}
<!-- Use the unminified version of T3 -->
<script src="./node_modules/t3js/dist/t3.js"></script>

<!-- Or -->

<!-- Use the minified version of T3 -->
<script src="./node_modules/t3js/dist/t3.min.js"></script>
{% endhighlight %}

Of course, you can also copy the files out of the npm package into another folder.

**Note:** T3 is designed to be used only in the browser, and as such, doesn't expose a CommonJS module for Node.js/io.js.

## Downloading from a CDN

You can also include T3 directly from a CDN by using [RawGit](http://rawgit.com). You can include a specific version of T3 by including the version number in the URL. For example. to use version 1.0.2, you can use the following:

{% highlight html %}
<!-- Use the unminified version of T3 -->
<script src="//cdn.rawgit.com/box/t3js/{{ site.data.t3.version }}/dist/t3.js"></script>

<!-- Or -->

<!-- Use the minified version of T3 -->
<script src="//cdn.rawgit.com/box/t3js/{{ site.data.t3.version }}/dist/t3.min.js"></script>
{% endhighlight %}

For development purposes, you can also link directly to the latest published version. This is not recommended in production because the contents of this file changes each time a new release is pushed:

{% highlight html %}
<!-- Dev-only: latest published release -->
<script src="//cdn.rawgit.com/box/t3js/master/dist/t3.js"></script>

<!-- Or -->

<!-- Dev-only: latest published release minified -->
<script src="//cdn.rawgit.com/box/t3js/master/dist/t3.min.js"></script>
{% endhighlight %}

**Note:** We highly recommend using a specific version of T3. Linking directly to the master branch means getting updates without notice.

## Which Installation Method is Right?

If you're unsure which installation method is right for you, it's best to start by downloading the file directly from GitHub and using it as you would any other dependency.