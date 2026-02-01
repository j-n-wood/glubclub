+++
date = '2026-02-01T14:22:14+13:00'
draft = false
title = 'Image orientation'
+++

# Incorrect image orientation

Surprise, something else behaving unexpectedly.

Photo from iphone in portrait.

In zed, views without using EXIF so is incorrect (on side) - or arguably correct as that is what is in the file.
In rendered locally via `hugo server`, is correct.
In image viewer, is correct.
Deployed, view in firefox - on its side. :sadface:
In chrome - same.

Now to learn how to strip the tags and rotate it properly.

Imagemagick: `mogrify -auto-orient -strip image.jpg`
