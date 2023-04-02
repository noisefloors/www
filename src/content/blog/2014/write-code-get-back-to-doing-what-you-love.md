+++
authors = ["Nicholas Young"]
date = "2014-06-26T00:00:00Z"
title = "Write Code and Get Back to Doing What You Love"
topics = ["Engineering", "Software", "JavaScript", "Talks", "The Machine"]
+++

A few weeks ago, I gave a talk at the [Chicago Node.js](http://www.meetup.com/Chicago-Nodejs) meetup about our technology stack for [The Machine](http://nicholaswyoung.com/work/machinefm). I've only been working with Node.js for a couple of months, but in that time, I've learned many difficult lessons. The biggest one, by far, is how *not to build a monolith*.

Rails (and many other web frameworks) work best if you follow the golden path. While I generally believe in convention-over-configuration, we need to recognize when certain conventions aren't right for our application. In this presentation, I detail why Rails (at least out of the box) didn't fit our needs. We needed a high-performance, fault-tolerant approach for the public CMS, feed rendering, and media analytics components in our system, but Ruby couldn't seem to deliver. Node.js seemed to fit the bill. However, to remain agile, I was forced to jettison previous "best practices" from other languages and learn the correct JavaScript idioms.

<iframe width="560" height="315" src="https://www.youtube.com/embed/xgsZCC10z2s" frameborder="0" allowfullscreen></iframe>

If you have questions, comments, or feedback of any kind, I'm always available on [Twitter](http://twitter.com/nicholaswyoung).
