---
layout: post # required
title: This is an Example Post # required
date: # date of post, time optional YYYY-MM-DD (HH:MM:SS)
description:  # Add post description for homepage - required
img:  # Add image to post - will be used as thumbnail on home and cover image for post (optional) MUST BE IN /img FOLDER.
fig-caption: # caption for img (optional)
tags: [One, Two, Three] # add tags within brackets separated by a commma (optional)
comments: True # must include. change to False if you want to turn comments off for a post
---


FOR IMAGES

<figure class="post-img XXX">
  <a href="/assets/img/posts/FOLDER/IMAGENAME">
    <img src="/assets/img/posts/FOLDER/IMAGENAME">
  </a>
  <figcaption>Macaroons!</figcaption>
</figure>

1. choose how you want the image displayed by replacing the XXX with one of the below three
- block
- left-inline
- right-inline

2. update the FOLDER and IMAGENAME
  - the <a> tag is a link to the picture. this is what lets you click/tap on the photo to make it bigger over the post.

3. add a caption (not necessary)

4. the figure tag to the post on it's own line. make sure to 'bundle exec jekyll serve' to check how it looks before posting
   - for RIGHT ALIGNED images, the text BEFORE the figure tag will be inline
   - for LEFT ALIGNED images, the text AFTER the figure tag will be inline
   - notice on /photo_change.html if there are 2 in a row with the same alignment with a small amount of text between, it will load wonky. If there was a longer paragraph there it would be fine, because the text area for the full length of the photo would be filled. but, because it's just a line or two, the next photo tries to align itself inline with the first photo and the text.
   - also - if there's a photo after the last part of text, it should be block. look at the /photo_change and the right-aligned one isn't working well. change that to block and it looks fine.
