# Octopress QR-Code in sidebar

This is a simple aside for <a href="http://www.octopress.org">Octopress</a> that uses the Google Code-API to automatic generate and dislay the QR Code of the actually visible page or post in the sidebar.

## Preview

Check my [blog](http://home-server-mind.com/automatische-qr-code-generierung-in-octopress/) for a preview in the sidbar and information in german.

## Setup

First of all you need to copy the file:

* *qrcode.html* into *source/_includes/custom/asides/*

After that you need to update these file:

### _config.yml

* add *'custom/asides/qrcode.html'* to *default_asides*

## That's it. More options:

## Option Change color

To change the color of the QR-Code-image substitute in file *qrcode.html* in the part
```
img src="http://chart.apis.google.com/chart?chs=100x100&cht=qr&chld=|0
&chco=0000FF&chl=...
```
```
&chco=0000FF
```
e.g. to
* red: &chco=FF0000
* green: &chco=00FF00
or any other color marked in hexcode (without the #).

## Option Change size

To change the size of the QR-Code-image substitute in file *qrcode.html* in the part
```
img src="http://chart.apis.google.com/chart?chs=100x100&cht=qr&chld=|0
&chco=0000FF&chl=...
```
```
100x100
```
in the size you want. It size is given in pixels (pt). Height and width must be the same, eg. 150x150, 200x200 etc.



## Additional note:
The word 'QR Code' is a registered trademark of DENSO WAVE INCORPORATED. It applies only for the word 'QR Code', not for image. I mention it in the abbr-tag in &trade;, so your are save with it.
