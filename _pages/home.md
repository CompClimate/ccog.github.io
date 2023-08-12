---
layout: splash
permalink: /
tagline: "at UC Davis"
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/footer-bahamas.jpeg
  caption: "Photo credit: [JPL/NASA](https://sealevel.jpl.nasa.gov/ocean-observation/why-study-the-ocean/overview/)"

---



# Improving ocean and climate understanding and resilience 

> We target grand challenges with the aim of improving ocean and climate understanding and resilience. Solutions to the challenges humanity, and the world, face are inherently interdisciplinary, and so is our lab. Blending cutting-edge computational and Earth science tools and knowledge, we combine theory, observations, and numerics to pioneer methods and create insight.

CCOG focuses on several research areas:


{% capture notice-1 %}
**Computational**: *Injecting knowledge to guide innovation*
  1. **Data mining:** Pioneer methods fit for purpose to uncover fundamental insight
  2. **Sparse data inference:** Leverage complicated and messy data
  3. **AI for science:** UQ and XAI for utilizing machine learning as universal function approximator
{% endcapture %}

{% capture notice-2 %}
**Earth Science**: *Objective advancement of our understanding of the Earth*
  1. **Fundamental insight**: Elucidate ocean and climate dynamics
  2. **Forecasting:** Improve predictions on long range weather and climate
  3. **Resilience:** Study impacts on physical and biogeochemical ocean and climate
{% endcapture %}

<div class="notice">{{ notice-1 | markdownify }}</div>
<div class="notice">{{ notice-2 | markdownify }}</div>


## Learn more

<div id="learn-more" class="videos__container"> 
  <div class="fluid-width-video-wrapper" style="padding-top: 49.9666%;">
    <iframe src="https://www.youtube.com/embed/20NnFCrCAj8" > </iframe>
  </div> 
  <a href="https://thirdpodfromthesun.com/2023/05/05/wave-and-means/">
    <img src="{{ site.baseurl }}/assets/images/thirdpod.png">
  </a>  
</div>

## News

{% assign sorted = site.news | sort: 'date' | reverse %}

<div id='short_news' style="display: block;">
  <ul>
  {% for news in sorted limit:5 %}
    <li><b> {{ news.date | date: "%y/%m" }} </b> - {{ news.content | markdownify  | remove: "<p>" | remove: "</p>"}} </li>
  {% endfor %}
  </ul>
  <a href="#" onclick="hideBlock('short_news'); showBlock('long_news'); return false;" class="btn btn--primary">Show more</a>
</div>

<div id='long_news' style="display: none;">
  <ul>
  {% assign sorted = site.news | sort: 'date' | reverse %}
  {% for news in sorted %}
    <li><b> {{ news.date | date: "%y/%m" }} </b> - {{ news.content | markdownify  | remove: "<p>" | remove: "</p>"}} </li>
  {% endfor %}
  </ul>
  <a href="#" onclick="hideBlock('long_news'); showBlock('short_news'); return false;" class="btn btn--primary">Show less</a>
</div>
