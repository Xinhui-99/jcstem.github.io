---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth:
title: "JC STEM Lab of MediaML @ HKU"

sidebar: right
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div class="row main-content" style= "margin-top: 30px; max-height:540px;">
  <div class="column small-9 pc">
    
    <!-- carrousel -->

    <div id="myCarousel" class="carousel slide" data-ride="carousel" style="">
        <!-- Indicators -->
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
        </ol>

        <!-- Wrapper for slides -->
        <div class="carousel-inner">
          {% include carousel_item.html  active="true" 
             url="" 
             image="images/images_for_pub/liu2025long.png" 
             alt="Improving Long-Text Alignment for Text-to-Image Diffusion Models" 
             title="Improving Long-Text Alignment for Text-to-Image Diffusion Models" 
             caption="This work investigates alignment diffusion models for long-text prompts using segment-level encoding and decomposed preference optimization." %}
            
          {% include carousel_item.html  
             url=""
             image="images/images_for_pub/li2024avideo.png" 
             alt="A Video is Worth 256 Bases: Spatial-Temporal Expectation-Maximization Inversion for Zero-Shot Video Editing" 
             title="Zero-Shot Video Editing" 
             caption="This paper presents a video inversion approach for zero-shot video editing, which models the input video with low-rank representation during the inversion process." %}

        </div>

        <!-- Left and right controls -->
        <a class="left carousel-control" href="#myCarousel" data-slide="prev">
          <span class="glyphicon glyphicon-chevron-left"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="right carousel-control" href="#myCarousel" data-slide="next">
          <span class="glyphicon glyphicon-chevron-right"></span>
          <span class="sr-only">Next</span>
        </a>
    </div>
  </div>

  <!-- carrousel on mobile devices -->
  <div class="column small-12 mobile">
    
    <!-- carrousel -->

    <div id="myCarousel" class="carousel slide" data-ride="carousel" style="">
        <!-- Indicators -->
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
        </ol>

        <!-- Wrapper for slides -->
        <div class="carousel-inner">
          {% include carousel_item.html  active="true" 
             url="" 
             image="images/images_for_pub/liu2025long.png" 
             alt="Improving Long-Text Alignment for Text-to-Image Diffusion Models" 
             title="Improving Long-Text Alignment for Text-to-Image Diffusion Models" 
             caption="This work investigates alignment diffusion models for long-text prompts using segment-level encoding and decomposed preference optimization." %}
            
          {% include carousel_item.html  
             url=""
             image="images/images_for_pub/li2024avideo.png" 
             alt="A Video is Worth 256 Bases: Spatial-Temporal Expectation-Maximization Inversion for Zero-Shot Video Editing" 
             title="Zero-Shot Video Editing" 
             caption="This paper presents a video inversion approach for zero-shot video editing, which models the input video with low-rank representation during the inversion process." %}

        </div>

        <!-- Left and right controls -->
        <a class="left carousel-control" href="#myCarousel" data-slide="prev">
          <span class="glyphicon glyphicon-chevron-left"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="right carousel-control" href="#myCarousel" data-slide="next">
          <span class="glyphicon glyphicon-chevron-right"></span>
          <span class="sr-only">Next</span>
        </a>
    </div>
  </div>

  <div class="column small-3 pc" style="max-height: inherit">
  	<div><h3>News</h3></div>

    <div class="list-group" style="margin-left=0; max-height: inherit; overflow-y: auto;">
    {% include news_item.html 
        highlight="true" date="Always"
        content="We are hiring! Several Ph.D. and master positions are now available in our group. Candidates with strong academic background and/or solid programming skills are highly preferred. Click <a href=\"recruitment\"><strong>here</strong></a> to see more details." %}

    {% include news_item.html  date="6-July-2025" content="Two papers are accepted to ACM MM 2025." %}
    {% include news_item.html  date="26-Jun-2025" content="One paper is accepted to ICCV 2025." %}
    {% include news_item.html  date="9-May-2025" content="One paper is accepted to ICLR 2025." %}

    </div>
  </div>
</div>

<div class="column small-12 mobile">
    <br>
    <h3>News</h3>
    <div class="list-group" style="margin-left=0; max-height: inherit; overflow-y: auto;">
      
    <!-- {% include news_item.html 
        highlight="true" date="Always"
        content="We are hiring! Several Ph.D. and master positions are now available in our group. Candidates with strong academic background and/or solid programming skills are highly preferred. Click <a href=\"recruitment\"><strong>here</strong></a> to see more details." %} -->

    {% include news_item.html  date="6-July-2025" content="Two papers are accepted to ACM MM 2025." %}
    {% include news_item.html  date="26-Jun-2025" content="One paper is accepted to ICCV 2025." %}
    {% include news_item.html  date="9-May-2025" content="One paper is accepted to ICLR 2025." %}

    </div>
    <h3 class="mobile"> About Us </h3>
    <b>JC STEM Lab of MediaML</b> @ HKU is founded in 2022. Our research focuses on endowing machines with the capability to perceive, understand, reconstruct, and interact with the visual world, with the following focuses:
    <ul> 
      <li>label-efficient, transferrable and lifelong machine learning algorithms that are generalizable to various visual tasks</li>
      <li>efficient compression techniques for visual data transmission</li>
      <li>effective techniques for perceiving, interpreting and reasoning multi-modal (including vision, language, etc.) knowledge</li>
      <li>learnable 3D models for extracting 3D semantics, inferring geometrical relationships, and rendering high-fidelity geometrical structures</li>
      <li>deeply learned generative models for synthesizing or translating between multi-modal data.</li>
    </ul>
</div>

---

<div class="pc" style="margin-left: 2%">
<b>JC STEM Lab of MediaML</b> @ HKU is founded in 2022. Our research focuses on endowing machines with the capability to perceive, understand, reconstruct, and interact with the visual world, with the following focuses:
    <ul style="margin-bottom:5px;"> 
      <li>label-efficient, transferrable and lifelong machine learning algorithms that are generalizable to various visual tasks</li>
      <li>efficient compression techniques for visual data transmission</li>
      <li>effective techniques for perceiving, interpreting and reasoning multi-modal (including vision, language, etc.) knowledge</li>
      <li>learnable 3D models for extracting 3D semantics, inferring geometrical relationships, and rendering high-fidelity geometrical structures</li>
      <li>deeply learned generative models for synthesizing or translating between multi-modal data.</li>
    </ul>
 The <b>JC STEM Lab of MediaML</b> is run by Prof. Dong Xu (IEEE & IAPR Fellow, Member of the Academia Europaea, Clarivate Analytics 2018 Highly Cited Researcher in the field of Engineering, Receipt of T-MM 2014 Prize Paper Award and CVPR 2010 Best Student Paper Award [with the PhD students supervised by Prof. Xu]) at the University of Hong Kong, Hong Kong.
</div>
