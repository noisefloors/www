+++
authors = ["Nicholas Young"]
categories = ["Design", "Dark Mode", "A11y", "Accessibility", "CSS", "HTML"]
date = "2020-07-06T00:00:00Z"
draft = false
illustrationDescription = "From the top, a dimly-lit escalator bathed in a red hue from reflected neon lights. Image courtesy of Scott Stefan on Unsplash."
layout = "post"
title = "Dark Mode on the Web: A Complete Guide"
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
Cox, [a professor of human-computer interaction at UCL, cautions against taking
popular assertions at face value][wired], telling *Wired* magazine "I'm not
aware of any robust evidence that white text on black background reduces eye
strain."

Examining dark mode through the lens of accessibility demonstrates that it is
beneficial to some while frustrating others. For example, while dark colored
backgrounds may reduce glare for certain users, further research reveals they
[may also cause highly interactive or animated interfaces to appear
blurred][ux-a11y], due to current [display manufacturing
techniques][wiki-motion-blur].

## Should I Implement Dark Mode?

It depends on several factors. If your site or application is either mobile-first
or attracts significant mobile traffic, I'd encourage you to consider it. One
study, ran by Google and focused on mobile devices using OLED screen
technology, found that dark mode consumes up to [60% less power when compared
to bright white themes][dark-mode-study]. This outcome is largely expected,
since OLED panels allow unused portions of the display (pure black) to be
completely powered off.

Similarly, while dark mode isn't an aid to every visitor, some will find it
useful. Most critical is properly detecting and adhering to user preferences
configured at the operating system level.

## Implementation

It's time to dive into code. During this exercise, we will do the following:

1. Detect whether a visitor has set their preferred color-scheme

As of this post, all major operating systems (including Linux) allow choosing
light or dark interface variants, which is then [exposed in CSS as the
`prefers-color-scheme` media feature][css-color-scheme].

2. Render a default theme based on the user's global preference

Whether the user has set preferences for light or dark, we should present
options for both. Many website

3. Allow visitors to override operating system configuration

Since accesibility is a very personal concern, we shouldn't require changing
operating system preferences. Instead, we should let users manually override
theme defaults, locally storing their choice to be loaded on the next visit.

[designshack]: https://designshack.net/articles/trends/designing-for-dark-mode/
[dark-mode-requirements]: https://css-tricks.com/lets-say-you-were-going-to-write-a-blog-post-about-dark-mode/
[aao]: https://www.aao.org/eye-health/tips-prevention/should-you-use-night-mode-to-reduce-blue-light
[wired]: https://www.wired.co.uk/article/dark-mode-chrome-android-ios-science
[css-tricks]: https://css-tricks.com
[ux-colors]: https://uxdesign.cc/dark-mode-ui-design-the-definitive-guide-part-1-color-53dcfaea5129
[ux-a11y]: https://uxdesign.cc/accessibility-and-dark-ui-themes-f01001339b65
[wiki-motion-blur]: https://en.wikipedia.org/wiki/Display_motion_blur
[dark-mode-study]: https://www.theverge.com/2018/11/8/18076502/google-dark-mode-android-battery-life
[css-color-scheme]: https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme
