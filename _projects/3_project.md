---
layout: page
title: Embedding with DWave
description: A small venture into the embedding statistics for a quantum annealer.
img: assets/img/CPCG_3.png
redirect: https://unsplash.com
importance: 3
category: work
---

A small dive into DWave's Pegasus QPU, as part of my first year in quantum computing. Involving a few weeks of training by post-doc staff at Purdue, I more or less stumbled my way into solving this problem and finding relations of Cartesian Product graph size and resource use. 

For context, a Cartesian Product graph is a pretty nifty way to represent bipartite graphs by splitting them into partitions, where all qubits (nodes) between partitions are fully connected. While these graph types are useful in their own right for network theory and simplifying graph structures, their nature allows them to be especially suited for an annealer processor which needs strict controls on embedding lengths / strengths. In fact, these structures allow problems to be tuned easier, and present an edge for industry to find the most use from annealers (in the future).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/CPCG_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/CPCG_2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The gist of my results - keep in mind that this was the culmination of many weeks of trial and error with a SLURM supercomputing environment. These trends show the resource scaling of embeddings for problems of size Kn, where n is the number of qubits to a partition. For example, K18 x K10 houses a bipartite graph of 180 logical qubits, but connections (couplings) require physical qubits, and embedding the entire structure therefore takes over 3000 physical qubits! 
