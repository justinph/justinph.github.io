---
layout: project
title: Audio Backpack
permalink: /projects/audio-backpack/
subhead: Music collection app, Winter 2014/2015
link: https://apps.classicalmpr.org/audio-backpack/
image: audiobackpack.png
excerpt: <p>Music educators have a difficult time finding sample audio to use in their classrooms and assignments. Minnesota Public Radio’s classical music staff knew how to help them, but needed a way to share their expertise and audio collection.</p> <p>This client-side app helps teachers create custom playlists for their classes and share them with students. </p> 

---

Music educators often have a difficult time finding music that is of good quality, easily aggregated, and not rights encumbered for use in their lessons. This web app aims to solve these problems.

The staff of Classical MPR has a wealth of knowledge about classical music and is very focused on music education. They identified and cut over 200 different segments of audio that exemplify different musical concepts. 

The web application I designed and built to share these clips and allow educators to search, save, and share them was based on [ember.js](http://emberjs.com/) and [bootstrap](http://getbootstrap.com/). This was one of the first true client-side only projects I have done; I went in a critic of this methodology and came away a believer. We use [prerender.io](prerender.io) to make sure that we send full HTML down the wire to sharing services and search engines. 

<img src="/images/audio-backpack/index.jpg" srcset="/images/audio-backpack/index-2x.jpg 2x"  alt="audio backpack home"/>

<img src="/images/audio-backpack/search.jpg" srcset="/images/audio-backpack/search-2x.jpg 2x"  alt="audio backpack search"/>

<img src="/images/audio-backpack/playlist.jpg" srcset="/images/audio-backpack/playlist-2x.jpg 2x"  alt="audio backpack playlist"/>

I worked with our back-end software developers to create a new playlist API that is used for this project. User accounts are created through a new [OAUTH2 service](https://accounts.publicradio.org/users/sign_in) that we set up. This service will be used for future projects to federate all user logins to one central service and will eventually be tied in with our CRM. 
