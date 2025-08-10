---
layout: page
title: Quantum Magic
description: Focused on discovering the relation between non-stabilizerness (magic) and barren plateaus.
img: assets/img/sre_ladder.png
importance: 2
category: work
giscus_comments: true
---

My newest venture, this project is lead by Myron Tadros and Prof. Andreas Jung. I have so far contributed in fashioning various metrics of non-stabilizerness (called 'magic' hereafter) for our specific needs. Because our project is concerned with the utility of magic and typical VQE circuits, we are comparing the runtime of their magic estimations for n qubits, k shots and m randomized gates. This is essential because different methods use different types of gates, different numbers of shots and work far worse for more qubits. This scaling determines what we regard as 'utility'.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sre_ladder.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sre_ladder_circuit.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div> <!--
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div> -->
</div>

<div class="caption">
    The left depicts magic, measured as Stabilizer Rényi-2 Entropy, over two variational angles linked by an entanglement ring. The two angles showed on the right 2dHist are theta_0 and theta_15, which represents the first P(0) and the last P(0) (or parameterized rotations) of the circuit. Keep in mind this is the layered circuit structure used by Qiskit.
(</div>

More information will be available as this science publishes this winter!

<!--
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>
-->

