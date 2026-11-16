---
title: kairos press kit
description: Fact sheet, descriptions, screenshots and the app icon for kairos.
---

<img src="{{ '/assets/apple-touch-icon.png' | relative_url }}" alt="kairos app icon" width="72" height="72" style="border-radius:16px">

# kairos press kit

kairos watches the forecast for the things you do outside and shows you the
best times to go: a low tide at sunset, a clean swell, a clear night for a
meteor shower. Most days it doesn't send a notification at all. There's no
account and no ads, and the app has no server of its own.

## Fact sheet

| | |
|---|---|
| **What** | An iPhone app that watches the forecast for what you do outside and shows the best times to go |
| **Platforms** | iPhone (iOS 17.6 and later). Android is in testing |
| **Price** | Free, no ads |
| **Coverage** | Tides, surf, rivers and topo maps: United States. Weather and the sky: anywhere |
| **Privacy** | No account, no analytics, no ads, and no server of its own. Settings and history stay on the phone ([privacy policy]({{ '/privacy' | relative_url }})) |
| **Accessibility** | Works with VoiceOver and the largest text sizes |
| **Developer** | Peter Overholser, Humboldt County, California |
| **Contact** | Through the [support page]({{ '/' | relative_url }}) |

## About

Good weather and a good time to go out aren't the same thing. A tidepooler
wants a minus tide in daylight. A surfer wants swell that reaches the break and
wind that stays down. A stargazer wants a clear night with the moon out of the
way. What counts as good depends on what you're doing, and a forecast doesn't
sort that out for you.

kairos does. You choose your activities and what you like for each one. It
scores the hours ahead and shows the best windows over the coming days. If a
window is unusually good, compared with the rest of the forecast and with the
days you've recorded, it sends a notification. Otherwise it stays out of the
way.

Running, walking, cycling, surfing, fishing, rafting and kayaking, skiing,
beachcombing, tidepooling and stargazing are built in, and you can add your
own. kairos works around your calendar and learns from how you rate your
outings. It warns you before a frost and before the year's highest tides. It
keeps offline topo maps that show where you are with no signal, with an arrow
that points back to your spot.

There's no account, and the app has no server of its own. Your settings,
history and ratings stay on your phone.

kairos is made by one person, Peter Overholser, in Humboldt County, California.
The name is the Greek word for the right moment.

{% assign shots = site.static_files | where_exp: "f", "f.path contains '/assets/press/'" | where: "extname", ".png" %}
{% if shots.size > 0 %}
## Screenshots

Real conditions on the north coast of California. Each opens full size.

<div style="display:flex;flex-wrap:wrap;gap:12px">
{% for shot in shots %}<a href="{{ shot.path | relative_url }}"><img src="{{ shot.path | relative_url }}" alt="kairos screenshot: {{ shot.basename | slice: 3, 40 | replace: '-', ' ' }}" width="180" style="border-radius:12px"></a>
{% endfor %}</div>
{% endif %}

{% assign videos = site.static_files | where_exp: "f", "f.path contains '/assets/press/'" | where: "extname", ".mp4" %}
{% for video in videos %}
## A short recording

<video src="{{ video.path | relative_url }}" controls playsinline width="300"></video>
{% endfor %}

## The icon

[512 px PNG]({{ '/assets/icon-512.png' | relative_url }}) ·
[512 px JPEG]({{ '/assets/icon-512.jpg' | relative_url }}) ·
[180 px]({{ '/assets/apple-touch-icon.png' | relative_url }})

## Coverage notes

Tide, surf, river and topo map data come from NOAA and USGS and cover the United
States. Weather and the sky work anywhere. kairos scores conditions against what
a person likes. It doesn't judge whether the ocean, a river or a slope is OK to
be on, and it says so in the app.
