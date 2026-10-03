---
layout: page
title: Personal
permalink: /personal/
---

I'm from [Northampton](https://en.wikipedia.org/wiki/Northampton,_Massachusetts), Massachusetts, a town known for its food, music and colorful folk. I'm the oldest of three, with two younger sisters, and spent my youth building forts in the woods behind our house, playing with Lego, jumping off dams, filming movies, and injuring myself learning to skateboard.

I moved to Boston for school in 2010 and met a wonderfully varied class of students, many of whom became lifelong friends. I ran along the Charles, ate very well at all hours, served as scholarship chair of my [fraternity](https://en.wikipedia.org/wiki/Sigma_Alpha_Mu) and president of the BU PC gaming club, and then went abroad on the [Geneva Physics program](http://www.bu.edu/abroad/programs/geneva-physics-program/), which started my career in particle physics. After graduating I stayed in the area for a job in Littleton, and spent my mornings and evenings reading on the commuter rail in and out of North Station.

In 2016 I moved to Los Angeles for graduate school and got used to the weather and the UCLA campus very quickly. Research on the LHC took me back and forth to Geneva (which didn't take much convincing) and introduced me to brilliant people from all over the world. In 2022 I came back to the Boston area to join Chloris.

## Outdoors

I spend as much time outside as I can, mostly rock climbing, snowboarding and hiking.

![Crans-Montana, Switzerland](/images/crans-montana.jpg)

## Travel

I've been lucky enough to travel much of the world, including more than two years living in Europe for my studies. I wrote up [a month-long trip around the world]({% post_url 2016-9-1-world-tour %}) and [a year in Geneva]({% post_url 2020-4-4-year-in-geneva %}) for anyone planning something similar. Some photos from along the way:

<div class="gallery">
{% assign photos = "angkor-wat.jpg:Angkor Wat, Cambodia|la-sagrada-familia.jpg:Sagrada Família, Barcelona|vevey.jpeg:Vevey, Switzerland|mont-serrat.jpg:Montserrat, Spain|shanghai.jpg:The Bund, Shanghai|grindelwald.jpeg:Grindelwald, Switzerland|buddha.jpg:Guanyin statue|cambodia.jpg:Temples near Siem Reap|yu-garden.jpg:Yu Garden, Shanghai|belvedere-palace.jpg:Belvedere Palace, Vienna|mammoth.jpeg:Mammoth Mountain, California|taj-mahal.jpg:Taj Mahal, Agra" | split: "|" %}
{% for p in photos %}{% assign parts = p | split: ":" %}
  <figure><img src="{{ '/images/' | append: parts[0] | relative_url }}" alt="{{ parts[1] }}" loading="lazy"><figcaption>{{ parts[1] }}</figcaption></figure>
{% endfor %}
</div>

## Music

I make music in Logic Pro now and then, and keep the outcomes I like on [SoundCloud](https://soundcloud.com/that-ivory).

## Magic: the Gathering

I'm a big fan of Magic and maintain a [Vintage Cube](https://cubecobra.com/cube/list/5f1de19a6ffa09102fca2040) that I update regularly.
