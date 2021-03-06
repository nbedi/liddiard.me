---
title: TypeEmoji
description: The no-nonsense emoji search keyboard
order: 11
link: http://typeemoji.com
involvement: creator
skills: React, ECMAScript 6, Sass, Amazon S3
github: liddiard/type-emoji
num_images: 4
---

Unicode emoji are all the rage these days – they're great for adding expression and flair to an online conversation, and they're supported almost everywhere. The hardest part of using them is finding the right one.

Plenty of websites exist for searching emoji, but they're most click farms that require annoying jumps between pages to get to the character you want to use. Apple Messenger and Slack have forms of emoji searching built in, but they're reliant on searching text in the emoji description.

I created TypeEmoji to make it easier to find the emoji you want quickly. It's a responsive, single-page React application with real-time emoji search. It searches not only on the official character descriptions, but also on additional "annotation" keywords provided by the Unicode Consortium. It orders search results by relevance.

I obtained the emoji data by parsing the [official emoji page from unicode.org](http://unicode.org/emoji/charts/full-emoji-list.html) with [kimono](https://www.kimonolabs.com).

Despite its simple interface, this application has some subtle features that make it work well, like only performing a search if there is significant duration between keystrokes to improve browser responsiveness, auto-selection of emoji on hover for copying, a visual highlight to confirm an emoji was copied to clipboard, and keystroke interception to ensure that typing always goes in the search input.