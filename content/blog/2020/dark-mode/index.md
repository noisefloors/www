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
mainstream design publications][designshack]. Maybe it's because a majority of
my work once took place after nightfall, but I've always favored dark color
palettes in UI design.

After noticing that trends were finally aligning with my preferred tastes,
I implemented user-selectable color schemes on this site; a process I found
unexpectedly difficult even after reading several articles on the topic. I'm
not alone in this observation: other design nerds have pointed it out too, most
notably Chris Coyier, [who listed out requirements for dark mode
tutorials][dark-mode-requirements] on his influential web design blog, [CSS
Tricks][css-tricks]. Much of the information you will find is valuable but
incomplete.

Like many emerging ideas on the web, implementing a dark color theme can be
complex because it exists at the intersection of several developing
technologies. Choosing the right tools to develop a solution is often
difficult, even for seasoned engineers.

## Demystifying "Dark Mode"

Fundamentally, implementing "dark mode" is swapping a bright, dark-on-light
color scheme for a light-on-dark version. This simple change brings several
proported health benefits; not the least of which is reducing our exposure to
[bright, direct light in the evenings][aao], and helps prevent disruption of
sleep cycles that is often associated with using screens before bed.

{{< figure src="ddg-dark-vs-light.png" title="DuckDuckGo's dark theme switches not only text and background colors, but highlight colors as well." >}}

As you might expect, this concept isn't entirely new. Software engineers have
long used low-brightness themes to combat fatigue and restlessness after
staring at a screen all day. However, as dark mode rises in popularity, the
overarching health benefits of adopting dark mode seem to be exaggerated. Anna
Cox, [a professor of human-computer interaction at UCL][wired], cautions taking
assertions at face value: "I'm not aware of any robust evidence that white text
on black background reduces eye strain."

Examining dark mode through the lens of accessibility demonstrates that it is
beneficial to some while frustrating others. For example, while dark colored
backgrounds may reduce glare, further research reveals they [may also cause
highly interactive or animated interfaces to appear blurred][ux-a11y], due to
current [display manufacturing techniques][wiki-motion-blur].


## Should I Implement Dark Mode?


After reading all of this, you may find yourself asking if dark mode is worthwhile. 

I admit, it's a question I wrestle with often, and

However, the health benefits of dark mode seem to be exaggerated. For
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
[aao]: https://www.aao.org/eye-health/tips-prevention/should-you-use-night-mode-to-reduce-blue-light
[wired]: https://www.wired.co.uk/article/dark-mode-chrome-android-ios-science
[css-tricks]: https://css-tricks.com
[ux-colors]: https://uxdesign.cc/dark-mode-ui-design-the-definitive-guide-part-1-color-53dcfaea5129
[ux-a11y]: https://uxdesign.cc/accessibility-and-dark-ui-themes-f01001339b65
[wiki-motion-blur]: https://en.wikipedia.org/wiki/Display_motion_blur
