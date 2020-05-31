---
layout: post
comments: true
title:  "Fast interations in machine learning"
excerpt: "Machine learning development feedback loop sucks. When I worked on web dev, I could almost always instantly looks at the result just by refreshing the browser but the same doesn't apply to machine learning..."
date:   2020-01-04 00:40:00 +0700
---

Machine learning development feedback loop sucks. When I worked on web dev, I could almost always instantly looks at the result just by refreshing the browser but the same doesn't apply to machine learning, where each component of your system could takes at least couple of minutes to load/process.

While initially doing things like loading pretrained word embeddings for a couple of minutes seems like OK it adds up to a really big amount of time just to see whether your current approach is correct or not.

Any changes to this system will takes another chunk of time to the point that you feel like you just keep waiting and waiting before even seeing the results.

This is a problem because ideally you want to ship things quickly to make sure that your system works with the other components that it needs to interacts with. Moreover, you will also need to get inputs either from other people on your team or even other teams whose work intersect with yours.

Looking back, this seems obvious but somehow I needed to remind of myself this over and over again: always start with the Mininum Viable Product (MVP) of your system! a system that uses the simplest model, smallest pretrained embeddings, basically the simplest version of every component. This is important so that you don't waste your time developing things that's doesn't even work to begin with and also present an opportunity to get feedback of your work.

So to recap:

1. Establish baseline quickly
2. Demo it out to get feedback while incrementally try to improve it.
