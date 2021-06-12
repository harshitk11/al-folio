---
layout: page
title: IP Protection
description: Towards Increasing the Difficulty of Reverse Engineering of RSFQ Circuits
img: /assets/img/OR-AND.jpg
importance: 5
---
Energy efficient supercomputers based on superconducting electronics (SCE) have been pursued for about six decades
and can operate at ultra-high speed (near THz frequencies) while consuming ultra-low power.

In this project, we introduce a camouflaging method to protect the Intellectual Property of superconducting electronics; specifically, rapid single
flux quantum (RSFQ) technology, from reverse engineering.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ 'assets/img/THREAT_MODEL.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    RSFQ design flow is shown on the top half (shaded green). The bottom half (shaded red) depicts the reverse engineering flow employed by the attacker.
</div>


 We develop RSFQ camouflaged units by applying the structural similarity of RSFQ standard cells. A defense using the designed camouflaged RSFQ cells is combined with obfuscation of the temporal distribution of inputs to the IC to increase the attacker’s effort to de-camouflage. The approach establishes the complexity class of RSFQ de-camouflaging and a model checker is applied to evaluate the strength of the defenses. These techniques have been evaluated on ISCAS’85 combinational benchmarks and the controllers of the OpenSPARC T1 microprocessor. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ 'assets/img/temporal_obfuscation2.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Proposed defense using camouflaged gates, (a) camouflaged flip-flop array, and (b) temporal distribution of inputs to the circuit required for its correct functionality (This is the secret key).
</div>

For a detailed report of the work, please refer to our [paper](https://ieeexplore.ieee.org/document/8663415).
