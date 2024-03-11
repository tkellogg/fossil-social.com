---
title: Announcing fossil-social.com
layout: post
post-image: "/assets/images/blog/peach-8103765_960_720.jpg"
description: Fossil is now available as a service, making it
  easy for you to get control over your social media.
tags:
- announce
---

It shouldn't take a lot of effort to stay up to date with industry news. You used to be
able to read headlines out of a single journal to keep track of what's happening in your
industry. But then a lot of the information moved online into social media networks and
it got harder to keep track of trends.

Facebook, Instagram, TikTok, etc. all have timeline algorithms that decide what you see 
and when. These are optimized for keeping you glued to the app. The longer they keep
you doomscroolling, the more ad revenue they'll get.

Today we're launching Fossil as a service. Fossil is also a timeline algorithm **(currently 
available only for [Mastodon][mast])**, but instead optimizes for your time by highlighting 
interesting content and letting you ignore everything else. It does that by grouping 
similar posts together:

![image of fossil](/assets/images/blog/fossil-index-preview.jpeg)

Each group is automatically curated by AI. Posts that are about similar things are grouped
together and labelled. You can easily understand the general composition of your timeline over
the last day, and skip over entire categories.


## Why a service?
Fossil is a [free open source project][gh]. However, it's a little tricky to setup. A lot of
the people who were most interested in using it were the least likely to be able to set it up, 
whether that be due to lack of time or skills. After all, the people most interested in
saving time are often the ones who don't have extra time to experiment.

Today, fossil is available as a paid service. Subscriptions are either $4/month or $42/year.
A subscription gets you:

* Seamless setup
* Web app accessible in your browser from anywhere
* Maintenance and automatic updates to the latest version

<a href="https://app.fossil-social.com/" 
  style="
  background-color: #5060b0;
  color: #dddddd;
  text-decoration: none;
  padding: 1rem;
  margin: 2rem;
  border-radius: 0.5rem;
  align-items: center;
  justify-content: center;
  display: flex;
  ">
  Go There Now
</a>

Of course, you can also use the open source version of fossil.

## Why Mastodon?
Mastodon is an open source social network, which makes it very easy to build on. Many of the other 
social networks have been closing down access to their API lately, which makes development
more difficult.

Mastodon also doesn't have a timeline algorithm, so adding a new innovative algorithm is seemless
and clean. For example, in Twitter/X, it's difficult to read your entire timeline and be sure
you've found all posts, because their own algorithm is limiting the content available.

Fossil might support other social networks in the future. [Tell us which ones your interested in.][sheets]


 [gh]: https://github.com/tkellogg/fossil/
 [mast]: https://joinmastodon.org/#getting-started
 [sheets]: https://docs.google.com/forms/d/e/1FAIpQLScHppU4PAAjxqkJSIqY78xxEdxAWnnryZKvWGvqcoxJBF9VeA/viewform?usp=sf_link
