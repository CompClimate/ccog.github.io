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

The group focuses on several research areas:


{% capture notice-1 %}
**Computational**: *trustworthy innovation*
  1. **Knowledge-guided & interpretable ML** Building physics into models so results can be explained and verified
  2. **Discovery from data** Unsupervised methods (e.g. NEMI) that surface meaningful structure with principled validation
  3. **Trustworthy prediction** Uncertainty quantification and explainable AI (XAI) to make neural networks guides to discovery
{% endcapture %}

{% capture notice-2 %}
**Earth Science**: *Understanding for resilience*
  1. **Ocean & climate dynamics** Circulation regimes, the Southern Ocean, monsoons, and ocean–atmosphere coupling
  2. **Forecasting:** Improve predictions on long range weather and climate
  3. **Ecosystems & impacts** Marine ecological provinces, fisheries, and biogeochemistry for resilient communities
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

{% assign sorted = site.data.news | sort: 'date' | reverse %}

<div id='short_news' style="display: block;">
  <ul>
  {% for news in sorted limit:5 %}
    <li><b> {{ news.date | date: "%y/%m" }} </b> - {{ news.text | markdownify  | remove: "<p>" | remove: "</p>"}} </li>
  {% endfor %}
  </ul>
  <a href="#" onclick="hideBlock('short_news'); showBlock('long_news'); return false;" class="btn btn--primary">Show more</a>
</div>

<div id='long_news' style="display: none;">
  <ul>
  {% for news in sorted %}
    <li><b> {{ news.date | date: "%y/%m" }} </b> - {{ news.text | markdownify  | remove: "<p>" | remove: "</p>"}} </li>
  {% endfor %}
  </ul>
  <a href="#" onclick="hideBlock('long_news'); showBlock('short_news'); return false;" class="btn btn--primary">Show less</a>
</div>
