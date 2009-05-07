# Voodoo Child CSS Reset

## About This Archive

This CSS reset was originally published on my blog in May 2009.  

Shortly after development of this reset, I discovered Twitter Bootstrap and abandoned my homebrewed CSS resets and frameworks in favor of this and, later, Foundation.  

This repository was created for archival purposes.

## Original Blog Post Description

I developed my own CSS reset a while ago, and I’m pretty happy with how it’s working, so I thought I’d share it.

The concept of a “CSS Reset” is embarrassingly new to me–I only read about them a month or two ago.  Of course, 90% of what a reset does, I have done manually for years, but I stupidly never thought of separating the styles out that way.  When I read about resets, I was initially turned off because many of them seem way too aggressive.  (Upon searching for validation, I indeed found that it I wasn’t the only to [dismiss resets](http://snook.ca/archives/html_and_css/no_css_reset/) as a [bad thing](http://meiert.com/en/blog/20080419/reset-style-sheets-are-bad/).)

I’m a stubborn person, but fortunately I seem to be capable of talking myself out of stubborn positions.  A week or two back, I decided to try out the use of a reset, to see (A) if I liked the setup, and (B) if it seriously borked any of my recent work.  Looking around, I didn’t find any that did exactly what I wanted a reset to do.  The closest was a reset unofficially credited to [Shaun Inman](http://www.shauninman.com/), although it appears to be itself modification of the popular YUI reset.  It was as good a place as any to start, so I began to flesh out my own personal reset script.  Here’s what I came up with:

> ### [voodoo.css](https://github.com/thomshouse/voodoo.css/blob/master/voodoo.css)

A few things my reset does differently:

- This is a reset…  and then some.  The new rules I set are too modest to consider a CSS framework by any means, but they do go beyond a standard reset.  For those who would prefer just the reset, just take out everything after the “Slight Return”. (Yes, I am a dork.)
- I do not set all headers to 1em.  Rather, I went with a mix of the W3C “default” values and a little common sense: It’s pointless for H5 and H6 to be smaller than 1em so, instead, I decrease their font-weights.
- I treat H1 differently than other headers.  The train of thought is that H1’s will most likely appear at the top of the page, and so will not require a top-margin value.  H2’s and beyond will appear in the middle of page content and will probably look better with some extra separation.
- I do not reset the default list styles.  Lists-as-layout are very popular now and rightfully so, but they’re still great for normal lists–like this one–too.  I do provide “block-list” and “inline-list” class declarations for quickly & easily achieving headless lists.  I’m not sure how useful they are, though…  I’ve already encountered a case of a list that will be displayed as block for screens, but inline for iPhone/mobile.
- I fiddle with the display of sup/sub tags.  This behavior is out there in other reset scripts, but unfortunately I did not save my source for this partiicular solution…  Sorry!

I hope this reset script might be of some use to others.  More importantly, I hope this might help to open some minds about reset scripts.  They really are just a set of tools we each can choose to use…  or not use.  But we can forge our own tools.  We can write our own resets to our liking, so why not?