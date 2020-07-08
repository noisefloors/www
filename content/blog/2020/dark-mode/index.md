+++
authors = ["Nicholas Young"]
categories = ["Design", "Dark Mode", "A11y", "Accessibility", "CSS", "HTML"]
date = "2020-07-06T00:00:00Z"
draft = false
illustrationDescription = "From the top, a dimly-lit escalator bathed in a red hue from reflected neon lights. Image courtesy of Scott Stefan on Unsplash."
layout = "post"
title = "Dark Mode: The Complete Guide"
summary = "It's easy on the eyes and sometimes, even on your battery. So how do you turn off the lights?"
+++

Since the last design refresh of this site, dark interfaces began to [appear in
mainstream design publications][designshack].

Maybe it's because a majority of my work once took place after nightfall, but
I've always favored dark color palettes. After noticing that design trends
were finally shifting darker, I implemented user-selectable color schemes;
a process I found unexpectedly difficult. I'm not alone in this observation:
other design nerds have pointed it out too, most notably Chris Coyier, [who
listed out requirements for dark mode tutorials][dark-mode-requirements] on
his influential web design blog, [CSS Tricks][css-tricks]. There's a lot of incomplete knowledge on the subject.

Like many emerging ideas on the web, "dark mode" can be complex because it
exists at the intersection of several developing techniques. Even for
seasoned engineers, choosing the right tools to develop a solution can be
difficult.

## What is "Dark Mode" Anyway?

The central principle of "dark mode" is swapping the dark-on-light color
palette that has become the norm in modern design for a light-on-dark version.
This has several proported benefits, not the least of which is reducing eye
strain. Software engineers have long used low-brightness themes for years to
combat fatigue and restlessness after staring at a screen all day.

![Dark mode](ddg-dark-vs-light.png)

Unfortunately, the health benefits of dark mode seem to be exaggerated. For
certain disabilities, dark mode improves the user's experience while it
degrades functionality for others. This is why detecting and adhering to system
preferences is critical. However, one area where dark mode triumphs is on
devices featuring OLED screens, which allow portions of the display to be
entirely powered-of when unused. Studies of the original Google Pixel
demonstrated a 63% reduce in power drawn from the battery when dark mode is
enabled.

If you're looking for a guide on choosing a color palette for your dark theme,
[UX Collective has a handy article][ux-collective] on the subject.

## Demo

## Implementation

[designshack]: https://designshack.net/articles/trends/designing-for-dark-mode/
[dark-mode-requirements]: https://css-tricks.com/lets-say-you-were-going-to-write-a-blog-post-about-dark-mode/
[css-tricks]: https://css-tricks.com
[ux-collective]: https://uxdesign.cc/dark-mode-ui-design-the-definitive-guide-part-1-color-53dcfaea5129
