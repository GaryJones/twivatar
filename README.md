# Twivatar

WordPress plugin that adds a shortcode that echos the current Twitter avatar for a username.

## Description

Adds twivatar shortcode. When also passed a Twitter handle as the name attribute, the plugin will get the current avatar from Twitter, and store the URL for 24 hours. It then echoes out an image.

A demo can be seen in the sidebar at [Bsktweetup.info](http://bsktweetup.info).
## Installation ##

### Upload ###

1. Download the latest tagged archive (choose the "zip" option).
2. Go to the __Plugins -> Add New__ screen and click the __Upload__ tab.
3. Upload the zipped archive directly.
4. Go to the Plugins screen and click __Activate__.

### Manual ###

1. Download the latest tagged archive (choose the "zip" option).
2. Unzip the archive.
3. Copy the folder to your `/wp-content/plugins/` directory.
4. Go to the Plugins screen and click __Activate__.

Check out the Codex for more information [installing plugins manually](http://codex.wordpress.org/Managing_Plugins#Manual_Plugin_Installation).

### Git ###

Using git, browse to your `/wp-content/plugins/` directory and clone this repository:

`git clone git@github.com:GaryJones/twivatar.git`

Then go to your Plugins screen and click __Activate__.

## Usage ##

### Shortcode ###

A basic example would look like this:

`[twivatar name="GaryJ"]`

Where _GaryJ_ is the twitter avatar to get.

**Attributes** (optional unless marked otherwise):

 * `name` - Twitter handle. Required.
 * `size` - One of 'mini', 'normal' or 'bigger' Default is 'normal'.
 * `link` - Whether to link the image to the profile page on Twitter. Default is true.
 * `linkclass` - class attribute value of the link. Default is none.
 * `rel` - rel attribute value of the link. Default is none.
 * `class` - class attribute value of the image. Default is none.
 * `title` - title attribute value of the image. Default is none.

`[twivatar name="Gamajo" size="bigger" class="alignright" rel="me"]`

## Frequently Asked Questions

### Can I amend how long the image URL is cached for?

Not yet. In a future version of the plugin, you will be able to. Current default is 24 hours.

### Can I change the default Twitter image?

Not yet. In a future version of the plugin, you will be able to. Current default is to use an image file called `no-twitter-image.png` in a folder called `images` in your active theme.
This image is only used if no image can be determined for the account. Either Twitter is down, or the account doesn't exist. If the account does exist, but has no image, then the default one that Twitter uses will be stored.

## Screenshot

![Example output of multiple twivatars](https://raw.github.com/GaryJones/twivatar/master/assets/screenshot-1.png)
_Example of output as seen on http://bsktweetup.info/_

## Credits

Built by [Gary Jones](https://twitter.com/GaryJ)
Copyright 2012 [Gamajo Tech](http://gamajo.com/)