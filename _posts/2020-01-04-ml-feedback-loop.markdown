---
layout: post
comments: true
title:  "ML Feedback Loop"
excerpt: "ML feedback loop sucks. When I worked on web dev, I could almost always instantly looks at the result just by refreshing the browser. The same doesn't apply to machine learning."
date:   2020-01-04 00:40:00 +0700
---

ML feedback loop sucks. When I worked on web dev, I could almost always instantly looks at the result just by refreshing the browser. The same doesn't apply to machine learning, where each component of your system takes at least a couple of minutes to load/process.

While initially doing things like loading pretrained word embeddings for a couple of minutes seems like OK it adds up to a really big amount of time just to see whether your current approach is correct or not.

Any changes to this system will takes another chunk of time to the point that you feel like you just keep waiting and waiting before even seeing the results.

This is a problem because ideally you want to ship it quickly to make sure that your system works with the other components that it needs to interacts with.

And to get input either from other people on your team or even other teams whose work intersect with yours.

Any improvements could be made afterwards after you nail down this MVP system: using simplest model, smallest pretrained embeddings, basically the simplest of every component so that you can see the result quick.

So to recap: establish baseline quickly -> demo it out to get feedback while incrementally try to improve it.

Rereading this seems like it's so obvious, but somehow I keep forgetting it 😕
