# flarum-imgur-upload v3 [![Packagist](https://img.shields.io/packagist/v/matteocontrini/flarum-imgur-upload.svg)](https://packagist.org/packages/matteocontrini/flarum-imgur-upload)

**flarum-imgur-upload** is a [Flarum](https://github.com/flarum/flarum/) extension that allows posting images in Flarum posts using [Imgur](https://imgur.com/) for image hosting.

## Features
With flarum-imgur-upload you can upload images to Imgur while writing your post, and the extension will automatically embed the images in your post. You can also paste from clipboard to upload an image file.

Opposed to [flagrow/upload](https://github.com/flagrow/upload), this extension:

- doesn't touch your database
- uses Markdown for including images
- doesn't wrap the image in a frame, nor does it crop the image
- uploads the image using only client-side code (without using server/bandwidth resources)
- allows you to stop using the extension whenever you want. Previously uploaded images will stay there forever

Compared to the original extension (matpompili/flarum-imgur-uplad), this extension:

- doesn't resize/change orientation of images. The raw file is uploaded to Imgur
- supports paste from clipboard
- has been rewritten to use Flarum components
- supports beta 8
- has a more polished UI

## Install

```
composer require matteocontrini/flarum-imgur-upload
```

## Configuration
Since **flarum-imgur-upload** uses Imgur API to upload your images, you will need an Imgur Client ID. To get one simply register to the [Imgur](https://imgur.com/) website, and register an application [here](https://api.imgur.com/oauth2/addclient).
You need to choose a name for your application (e.g. My Forum), and select *OAuth 2 authorization without a callback URL*.

Once your application has been registered, your Client ID will be available [here](https://imgur.com/account/settings/apps). Simply put it in the configuration of the extension, in your admin page.

## Usage
When writing/editing a post click on the image button.

![DemoGIF](https://i.imgur.com/WtqxH4E.gif)
