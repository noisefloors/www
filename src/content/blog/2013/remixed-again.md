+++
authors = ["Nicholas Young"]
topics = ["design-refresh", "content-management", "personal-branding"]
date = "2013-04-11T00:00:00Z"
layout = "post"
path = "/remixed-again"
title = "Remixed, Again"

+++

I redesign this site annually, but this iteration is radically different. Normally, I pick a new set of technical tools and work around any associated oddness they might introduce &mdash; however, this time, I decided to be bold. I reimagined my personal design language, employed a simple file-based CMS, and picked a new hosting provider. Like I said, bold.

However, this post isn't about technical details alone. It's part of a (link: /notebook/its-not-about-your-tools text: much larger narrative) on choosing the right tools: ones that help you create better work. Even familiar tools will sometimes slow you down, and hinder creativity. Never be afraid to open your toolbox and replace pieces that don't work well for you.

## Design Language

Design is art and science, wrapped together in a single, cohesive package. Colors, font choices, line spacing, and menu structure are all crucial steps in this careful dance. Design language is a term coined to reflect the collective effect of each decision, and it's impact on the viewer.

If I choose the wrong font or size it incorrectly, my message is garbled. When in the studio, I ensure the vocalist can be heard, and this is no different. In fact, it could be even more important. The web is full of poorly designed sites, and their message suffers as a result. If a viewer cannot easily read my content, then they'll leave. I know my audience: you don't surf aimlessly and land here. Any visit is intentional, and I should treat you with respect.

For this redesign, I stripped my layout bare, only including essentials: clean typography, a bit of blank space, and simple navigation. I decided upfront to nix any extraneous elements: everything I added should provide value to the viewer. Headlines and body copy are set in (link: http://www.myfonts.com/fonts/canadatype/gibson text: Gibson), a beautifully straightforward sans-serif font designed by Rod McDonald, and distributed by Canada Type. I tried to keep colors minimal, and use the header (when appropriate) to showcase some of my recent photographic work.

The new minimalist logo tosses out everything but my first initial and two colors. I might change it in the future, but it will work nicely for now.

## Content Management

Beautiful design is nothing without content. It's something we, as designers, are often frustrated by, but understanding the end-user's content is a prerequisite for most design projects. Another universal truth is this: if managing content is difficult, the content will remain static. This is a lesson I've learned many times over; sometimes leaving this site untouched for a year or more.

Choosing the right content management system is a difficult proposition. In the past I've used traditional systems like (link: http://wordpress.org text: Wordpress) or (link: http://drupal.org text: Drupal), but tired quickly of the sometimes complex database maintenance tasks and upgrade procedures.

This site is powered by (link: http://getkirby.com text: Kirby); a small, eloquent framework that works without MySQL (the only requirement is PHP). At first, it sounded almost too simple, but I dove in, finding a robust content management engine that allows me to write in (link: http://daringfireball.net/projects/Markdown text: Markdown), and even add structured data. The whole site is (link: https://github.com/nicholaswyoung/web text: stored in a Git repository), and deployed from the command line. While a simple flat-file system like (link: http://getkirby.com text: Kirby) isn't ideal for every site, it allows me to build faster and write more often.

## Layout

Well over a decade ago, I opened Notepad and authored the first version of this site. It was a mess, with inline-styling and HTML break tags. Since then, CSS evolved from a minor help to formidable styling force &mdash; but even in 2013, it isn't perfect.

To remove repetitive stylesheet statements, I wrote most of the styles using Sass &mdash; or (link: http://sass-lang.com text: _Syntactically Awesome Stylesheets_). Sass extends CSS, adding support for nesting style declarations, mixins, and extension of existing statements. All markup is valid HTML5, a cleaner, grownup version of HTML4.

## Future Plans

This site isn't complete: there are still several additions I have planned, including (but not limited to) a photography portfolio, testimonials from clients, and sample audio clips for tracks I've mastered over the years. They will all arrive in due time, once I've completed the design for each section, and implemented it in a clean, maintainable fashion.

This site is radically different from it's predecessors, I said, and looking over the text above, I believe that is truer than ever. I chose a wholly new set of tools, and crafted something beautiful. I believe moving forward will be much easier thanks to these choices.

I charge you: carefully consider each new tool you add to your workflow, and never choose ones that will hinder your creative flow. It's easy to pick new, shiny tools without truly understanding how they affect your creative output. Be wary of ones that don't fit your personal creative process, and always be willing to toss out ones that frustrate you.
