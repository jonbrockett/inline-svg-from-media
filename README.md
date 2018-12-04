# Inline SVGs from WordPress Media Library
Embed SVGs as native HTML from the WordPress media library using a collection of custom functions.

_NOTE: This does not add support for SVGs in WordPress. You will need a plugin for this._

## Purpose
This is a collection of functions that are to be used instead of wp_get_attachment_image, etc. It detects the MIME type of the called attachment file. If it detects an SVG it uses __file_get_contents__ to display the raw SVG code (Make sure your SVGs are safe before you consider using this).

## Why Not Use JS?
Placing SVGs inline as HTML has a lot of benefits:
* They won't be another resource to call on load
* You can work with the code for animations, changing the fill color, etc.
* You don't need JS to convert the loaded image into inline code (preventing flashing among other things)
* They load VERY quickly since they are HTML

## About


## Requirements
I highly recommend using https://wordpress.org/plugins/safe-svg/ (This plugin is great for sanitizing malicious code which let's you open this up to allow SVG uploads from all roles)

## Functions
