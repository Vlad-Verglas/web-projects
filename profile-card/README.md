# Profile Card (Beta)

The beta version of this project is called "profile card".

The inspiration came from an exercise on freecodecamp.org, which helped me understand HTML. I am currently studying CSS, so the theme of the page, and the code itself, may change many times with future updates.

The goal of this page is to have a profile card directly online on the web. For now it has no real domain, but I will add an HTML anchor to link my future websites back to this one, to promote myself and to point back to the copyright. By the time you see this project online, the code will probably be published on GitHub as well.

I am changing my name across all my social media, because I wanted something more unique and generic. The new name is Vlad Verglas, and you can already see it on this profile card.

Now let's talk about the website.

## HTML

We start with the declaration (`<!DOCTYPE html>`). Then, in the `<html>` element, we add the `lang` attribute, which identifies the language used in the website.

In the `<head>` we put the `<meta>` elements needed for SEO, character encoding, and accessibility, then the title, and finally the void `<link>` element, which tells the browser that the `styles.css` file contains the style of the whole page.

We then add a `<div>` element with the ID `profile-card`. We use an image as a logo, instead of just a profile picture taken from the web: it is a monogram of my name, made of two V letters that form a single symbol. On line 13 we add a `<span>` element so that the name does not appear next to the profile picture.

Finally, we add the favicon and the description for SEO.

## CSS

In the CSS we start with the `body`: we set a background that is not too black, and a white-gray text color. In the `profile-card` ID we add a dark gray color, which creates the actual presentation of the card.

We resize both the image and the `profile-card` ID to center it on the page, so that the image is well framed inside the card. While experimenting with the radius, I found the `border-radius` property. I set it to 50% and I think the profile picture looks really great this way.

I did not write much CSS, and I probably still need to fix many things, but this is what I can do with CSS at the moment. I would like to study new features first, and then update this page and create other websites in the meantime.

## Final notes

This is my first documentation, so I apologize if it looks a bit unprofessional. It was translated from Italian to English with Claude AI. I am improving my English and I can already read it, but I did not feel ready to write my first documentation directly in English. Next project/update, I will.

Copyright (c) 2026 Vlad Verglas. All Rights Reserved.
