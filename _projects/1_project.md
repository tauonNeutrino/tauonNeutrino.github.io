---
layout: page
title: Image Metrology
description: An internship in Dortmund, DE led me to developing my skills in image metrology and software engineering. My most intensive project in coding, the support I received from my supervisors helped me increase the resolution and detection capabilities of their software near tenfold.
img: assets/img/R2_48_2_o_rescaled.png
importance: 1
category: work
related_publications: false
---

Over the course of that summer, I was involved in nearly all aspects of Dortmund's sensor preparations for ATLAS phase II. I enjoyed most helping to functionalize the coldbox (used for temperature cycling) through repairs and software functionality to measure the Euler angles of the sensor in any given scan. This was very useful for gaining more precision in sensor dimensions, and in understanding the construction process per chip.

The significance of this was to ensure that in the future, all fabricated sensors that TU Dort. would produce are up to a tight standard of construction. Any tiny sensor defect could balloon into missed weeks of collision time and over thousands of dollars lost. Sensor curvature, warping and misplaced components all contribute to lost science at some level.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/R2_68_1_h.jpg" title="A height subtraction transformation to cut out unnecessary information." class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/upper_strip_template.png" title="An example of template matching with OpenCV that was used to determine pixel ratios between different images." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: A height subtraction transformation to cut out unnecessary information. Right: An example of template matching with OpenCV that was used to determine pixel ratios between different images.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/R2_48_2_o_rescaled.png" title="Full image of a R2 radial strip sensor." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A colorless scan of the R2 sensor module. These are typically arranged in cylindrical slices around the beam axis, with R2 signifying closer to collisions than R5.
</div>

As the project came to a close, I found that I was most helpful with matching by angles. In OpenCV, it is quite easy to take a small template image and match it against the image of interest. The distribution of correlations can be shown, where the maximum corresponds to the angle of the reference image. By cross referencing different parts of the image of interest, we found small differences in angles, indicative of an imperfect production of that sensor. Finally, we got our measurement precision below the thresholds set by CERN!

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A display of measurement variance with our image matching techniques. The threshold is 100 microns, which greatly encompasses our values as the y axis in both module classes!
</div>

