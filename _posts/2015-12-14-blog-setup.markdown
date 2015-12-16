---
layout: post
title:  "Blog Setup"
date:   2015-12-14 14:24:44 -0800
categories: jekyll update
---

Since this is the first blog post it's almost necessary to describe how I set this up using [Jekyll][jekyll-docs]. Go to the link to learn about Jekyll, a blog-conscious tool for building a website. This post will also cover some information on getting your own email and setting up your own domain. 
<!--more-->

## The Basics 

A dear friend of mine in the bioinformatics program already has written a nice and brief post on using Jekyll and Github pages. Check out [her blog post][csiu-blog] on how she set up and customize her blog. She also has an awesome About page btw ;)  For a longer version of how to use Jekyll to set up your own website for free, see [here](http://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/).

## Customize the URL

My blog is different from my friend's blog in the way that I don't have any theme (simply the default Jekyll one) and I am using a custom domain name. To get a custom domain, simply purchase a domain name through [Namecheap (with my referral code)](https://www.namecheap.com/?aff=93243). Then follow [these steps](https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages) to create a CNAME file in your Github repo and configure your DNS in Namecheap to link it to your username.github.io pages. 

### Get a customized email address

You already paid for a domain name, so might as well get the most out of it. In the footer of this page, you can see that I also have an email address using my domain name. Instead of paying extra money to get that, you can simply [hack Gmail to use custom domains for free](https://simplyian.com/2015/01/07/Hacking-GMail-to-use-custom-domains-for-free/) by signing up for Mailgun and do some simple configuration in Gmail. 

When someone send me an email through my @santina.me email address, it actually goes to my Gmail. I can also send email using that email address in my Gmail. With Mailgun, you can set up as many different addresses as you like, such as "sup@santina.me" for general purposes or "connect@santina.me" for more serious stuff. With Gmail, you can then filter those emails. 

## Customize your own layout 

I'm new to Jekyll so rather than using a premade theme, I decided that it'd be a fun learning experience to investigate how to use Sass, a fancy version of CSS, and to see how everything is organized and configured in Jekyll. 

There are things you can add to a vanilla Jekyll blog, such as tags/topics and discussion board. See [this blog by Bruno][bruno-blog], who is also creating a blog to write posts to save people's time and have done quite some customizations with the layout and added features. I will be using his Github commits as guidelines on how to do the same for my blog. 

[jekyll-docs]: http://jekyllrb.com/docs/home
[csiu-blog]: http://csiu.github.io/update/2015/09/13/blog-setup.html
[dean-blog]: http://deanattali.com/
[bruno-blog]: http://bgran.de/

