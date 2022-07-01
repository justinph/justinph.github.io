---
layout: project
title: The New York Times
permalink: /projects/nytimes-dot-com/
#directlink: true
subhead: Various web projects, 2015&ndash;Present
#link: http://www.nytimes.com/books/best-sellers/
image: bestsellers.jpg
excerpt: <p>At The Gray Lady, I've worked on many different web projects. Currently, I work on technical SEO and social work with a focus on front-end presentation.</p>

---

Here lies a smattering of projects from my tenure at the New York Times.

## [Web Archive](https://archive.nytimes.com/)

<img src="/images/webarchive.jpg" alt="screenshot of nytimes web archive landing page" />


In 2016, the New York Times still ran its web site from servers it physically owned, slotted into racks in datacenters. We wanted to transition to The Cloud, but the physical servers still housed many old web pages that were important to preserve. I led a year-long effort to save and migrate those pages to an archive. This let us retire our physical datacenter and move all our digital products to the cloud. The archive has grown over time as additional projects have been shut down and the static content saved into the web archive.

* Example archive: [NYT Homepage on September 12, 2001](https://archive.nytimes.com/www.nytimes.com/indexes/2001/09/12/)
* [Slide deck with more details](https://www.slideshare.net/justinph/nyt-web-archive/justinph/nyt-web-archive)


<br />

## Preventing Social Misinformation

<img src="/images/socialcards.jpg" alt="screenshot of social sharing card with 2016 timestamp" class="medium" />


<!-- <img src="https://static01.nyt.com/images/2019/06/13/us/politics/13biden-abortion1/13biden-abortion1-facebookJumbo.jpg?year=2019&h=550&w=1050&s=edf80f913129db0400e1148f68d5539dddd954113b80616c9c2deb561c29ff6e&k=ZQJBKqZ0VN" /> -->

After the proliferation of misinformation during the 2016 U.S. election, we became concerned about the potential for misuse of our published content. Our chief concern was people re-posting older stories as new and readers not understanding that they were many years old. [Inspired by The Guardian](https://www.theguardian.com/help/insideguardian/2019/apr/02/why-were-making-the-age-of-our-journalism-clearer), we visually timestamped the sharing graphic for all our stories published over a year ago. This work was done in our CDN, [Fastly](https://developer.fastly.com/reference/io/), with some neat tricks to cryptographically ensure that the timestamp cannot be corrupted. Here's an [article about the feature on Poynter](https://www.poynter.org/ethics-trust/2022/news-orgs-mark-old-articles-disclaimer/).


<br />

## [HTML Sitemap](https://www.nytimes.com/sitemap/)

<img src="/images/sitemap.jpg" alt="screenshot of nytimes sitemap web page" />

As part of my team's work on SEO, we re-wrote the our XML sitemap to work seamlessly and accurately with our distributed publishing system. However, we didn't initally update our HTML sitemap. With this simple but useful project, we did just that.

The HTML sitemap is a simple list of every date the Times has been published, listing and linking to every piece of content ever published. Just simple, linked lists for humans and search engine robots.

[Example page](https://www.nytimes.com/sitemap/2020/03/17/)

<br />

## HSTS

<img src="/images/hsts.jpg" alt="screenshot of padlock icon from firefox" class="small" />


In the summer of 2020, another engineer and I decided we should continue the long process of making nytimes.com more secure. We used our [Maker Week](https://open.nytimes.com/innovating-from-home-maker-week-at-the-new-york-times-50ecfa38aca1) to enable [strict transport security](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security) on www.nytimes.com. This work won us some nice internal 👀 and also was a thing that helped us sleep easier at night.

A small nerd detail: we have intentionally _not_ turned on HSTS for all subdomains since archive.nytimes.com serves some content that cannot be upgraded to HTTPS.

<br />

## Gift Article Sharing

<img src="/images/giftarticle.jpg" alt="screenshot of gift article sharing menu" class="small" />


This feature allows paid subscribers of the Times to send links to their family or friends, allowing them to read them without a subscription. In essence, users can create URLs that bypass the NYT paywall. I lead the surprisingly intricate frontend development work on this project, working with other engineers who did the backend work. We conducted at least half a dozen A/B tests on this feature, each leading to increases in engagement and use.


<br />

## Rich Sharing

<a href="https://twitter.com/justinph/status/1529871122099060738"><img src="/images/tweet2.jpg" alt="screenshot of tweet with crosswords puzzle score" class="up-1" /></a><a href="https://twitter.com/justinph/status/1518609584201547778"><img src="/images/tweet1.jpg" alt="screenshot of tweet with quote from article" class="up-2" /></a>

Many digital products do not give readers a way to share all their activity or achievements. Users often execute workarounds by sharing screenshots of their crossword solve time, a paragraph they find interesting, or a map that shows something interesting. We have been experimenting with a mechanism that allows users to share these things without the need for cumbersome screenshots.

Try sharing these URLs: (right click, copy url)
* [Mini crossword win](https://www.nytimes.com/badges/games/mini.html?d=2022-04-26&t=72&c=e41f875b3c5dcfa5065c32b94b4250c5)
* [Astounding quote graphic](https://www.nytimes.com/shared/v0/2021/07/21/us/american-life-expectancy-report.html/01.html)


<br />

## Accessibility

Accessibility (a11y) has been a passion project of mine at the NYT. By organizing our internal accessibility community of practice, I try to support other staff who are interested in improving accessibility of their work. We have bi-weekly office hours and occasional talks on accesibility subjects.

When teams or projects ask, I am happy to conduct ad-hoc accessibility reviews and have even been known to submit pull requests with a11y improvements to codebases that I don't typically work in.



<!--

<br />

## /r/Coronavirus Bot

<br />

## Telegram Bot


<br />

## Visual Regression Testing

-->