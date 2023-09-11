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

#slider:
#text_color: white
#shadow_color: black
#slides: 
#  - image: gallery-example-1.jpg
#    slide_html:
#  - image: gallery-example-2.jpg
#    slide_html: "<h2>Yes, this carousel supports html texting</h2>"
#  - image: gallery-example-3.jpg
#    slide_html: "<h2>Yes, this carousel supports html texting</h2>"

sidebar: right

# widget1:
#   title: "GradNet ICCV2019 Demo"
#   url: 'https://youtu.be/tWDbs3VrnbU'
#   video: '<iframe width="360" height="240" src="https://www.youtube.com/embed/tWDbs3VrnbU" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="max-width: 100%; max-height: 150pt;"></iframe>'
#   text: 'Check out our demo for Visual Object Tracking'
# widget2:
#   title: "Video Tracking"
#   url: 'https://www.youtube.com/watch?v=M1LqUV4jLbM'
#   text: 'Implementation of MDNet, KCF and SiamFC.'
#   video: '<iframe src="https://www.youtube.com/embed/M1LqUV4jLbM" width="360" height="240" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="max-width: 100%; max-height: 150pt;"></iframe>'
# widget3:
#   title: "Pose Tracking"
#   url: 'https://youtu.be/CiKJuAH2U8I'
#   video: '<iframe src="https://www.youtube.com/embed/AL-8XCzRFo0" width="360" height="240" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="max-width: 100%; max-height: 150pt;"></iframe>'
#   text: 'Our team won the 2nd place in the pose-track challenge.'

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
             image="images/images_for_pub/brnet2021.png" 
             alt="3D Object Detection in Point Clouds" 
             title="3D Object Detection in Point Clouds" 
             caption="We introduce a new 3D object detection method, named as Back-tracing Representative Points Network (BR-Net), which generatively back-traces representative points from the vote centers and revisits complementary seed points around these generated points, so as to better capture the fine local structural features surrounding the potential objects from the raw point clouds. " %}
            
          {% include carousel_item.html  
             url=""
             image="images/images_for_pub/3D_Det.png" 
             alt="DVC: An End-to-end Deep Video Compression Framework" 
             title="Accurate Monocular 3D Object Detection" 
             caption="we propose a monocular 3D object detection framework in the domain of autonomous driving. Unlike previous image-based methods which focus on RGB feature extracted from 2D images" %}

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
             image="images/images_for_pub/brnet2021.png" 
             alt="3D Object Detection in Point Clouds" 
             title="3D Object Detection in Point Clouds" 
             caption="We introduce a new 3D object detection method, named as Back-tracing Representative Points Network (BR-Net), which generatively back-traces representative points from the vote centers and revisits complementary seed points around these generated points, so as to better capture the fine local structural features surrounding the potential objects from the raw point clouds. " %}

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

    <!-- {% include news_item.html  date="23-July-2021" content="Three papers are accepted to ICCV 2021." %} -->

    <!-- {% include news_item.html  date="10-July-2021" content="Two papers are accepted to ACM MM 2021 with one Oral." %} -->

    <!-- {% include news_item.html  date="4-March-2021" content="Five papers are accepted to CVPR 2021 with three Oral and two Poster." %} -->

    <!-- {% include news_item.html  date="4-July-2020" content="Five papers are accepted to ECCV 2020 with three Oral (2%) and two Poster." %} -->

    <!-- {% include news_item.html  date="30-May-2020" content="One paper is accepted to IJCV." %} -->

    <!-- {% include news_item.html  date="20-April-2020" content="One paper is accepted to TPAMI." %} -->

  	<!-- {% include news_item.html  date="1-Sep-2019" content="Our lab established!" %} -->

    </div>
  </div>
</div>

<div class="column small-12 mobile">
    <br>
    <h3>News</h3>
    <div class="list-group" style="margin-left=0; max-height: inherit; overflow-y: auto;">
      
    {% include news_item.html 
        highlight="true" date="Always"
        content="We are hiring! Several Ph.D. and master positions are now available in our group. Candidates with strong academic background and/or solid programming skills are highly preferred. Click <a href=\"recruitment\"><strong>here</strong></a> to see more details." %}

    <!-- {% include news_item.html  date="23-July-2021" content="Three papers are accepted to ICCV 2021." %} -->
    
    <!-- {% include news_item.html  date="10-July-2021" content="Two papers are accepted to ACM MM 2021 with one Oral." %} -->
    
    <!-- {% include news_item.html  date="4-March-2021" content="Five papers are accepted to CVPR 2021 with Three Oral and two Poster." %} -->

    <!-- {% include news_item.html  date="4-July-2020" content="Five papers are accepted to ECCV 2020 with Three Oral (2%) and two Poster." %} -->

    <!-- {% include news_item.html  date="30-May-2020" content="One paper is accepted to IJCV." %} -->

    <!-- {% include news_item.html  date="20-April-2020" content="One paper is accepted to TPAMI." %} -->


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
 The <b>JC STEM Lab of MediaML</b> is run by Prof. Dong Xu (IEEE & IAPR Fellow, Clarivate Analytics 2018 Highly Cited Researcher in the field of Engineering, Receipt of T-MM 2014 Prize Paper Award and CVPR 2010 Best Student Paper Award [with the PhD students supervised by Prof. Xu]) at the University of Hong Kong, Hong Kong.
</div>
