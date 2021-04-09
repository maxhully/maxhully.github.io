---
layout: post
title: Some Mapbox GL JS performance tips
---

I've been using Mapbox GL JS extensively for basically my entire career.

Here are some easy tweaks you can implement to improve the performance of your
Mapbox web maps:

- Pass the URL for GeoJSON layers instead of fetching the GeoJSON yourself
- Use `Promise.all()` when fetching multiple layers
- Remember: paint properties > layout properties > filters (I think)
- Vector tile layers perform better than GeoJSON layers
- Consolidate your event handlers
