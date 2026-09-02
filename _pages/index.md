---
layout: single
permalink: /
cssclasses:
  - wide
author_profile: true
header:
  overlay_image: assets/images/uk-bristol-bridge.png
  overlay_filter: 0.3
  show_overlay_excerpt: true
excerpt: __Climate modeller.__
title: Dr Dan Skinner
---
# Hi, I'm Dan!
<img style="float:right;width:300px;padding:10px;border-radius:10px" src="assets/images/cornwall.jpeg">
*I'm climate scientist at the University of Bristol, working with the HadCM3B-ESM model to study detection and attribution, with particular focus on human health impacts.*

My current work forms part of the wider [BREATHE](_pages/research/#BREATHE) project, a large consortium studying the attribution of climate-related health outcomes to human emissions. 

Whilst I currently work with the HadCM3B-ESM model at the University of Bristol, I also have experience running the IGCM4 model at the University of East Anglia where I spent a number of years. 

<div style="text-align:center;">
{% include button.html button_name="Find out more" button_class="large" url="/research" %}        {% include button.html button_name="Get in touch" button_class="large" url="contact" %}
</div>

{% assign latest_post = site.posts.first %}

{% if latest_post %}
<div class="latest-news-box" style="border: 1px solid #ddd; padding: 20px; border-radius: 8px; margin: 20px 0; background-color: #f9f9f9;">
  <span class="news-badge" style="background-color: #d32f2f; color: #fff; padding: 3px 8px; font-size: 0.75rem; font-weight: bold; border-radius: 3px; text-transform: uppercase;">Latest News</span>
  
  <h3 style="margin: 10px 0 5px 0;">
    <a href="{{ latest_post.url | relative_url }}" style="color: #333; text-decoration: none;">{{ latest_post.title }}</a>
  </h3>
  
  <p class="news-date" style="color: #666; font-size: 0.85rem; margin-bottom: 12px;">
    Published on {{ latest_post.date | date: "%B %d, %Y" }}
  </p>
  
  <div class="news-excerpt" style="font-size: 0.95rem; line-height: 1.5; margin-bottom: 15px;">
    {{ latest_post.excerpt | strip_html | truncatewords: 20 }}
  </div>
  
  <a href="{{ latest_post.url | relative_url }}" class="read-more" style="display: inline-block; font-weight: bold; color: #d32f2f; text-decoration: none; font-size: 0.9rem;">
    Read Article &rarr;
  </a>
</div>
{% endif %}
