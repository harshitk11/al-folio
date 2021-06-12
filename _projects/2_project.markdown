---
layout: page
title: Power Management based Malware Detector
description: Securing IoT Devices using Dynamic Power Management
img: /assets/img/Fig1_v4-1.jpg
importance: 4
---
In this work, we demonstrate that Dynamic Voltage and Frequency Scaling (DVFS) states form a signature pertinent to an application, and its run-time variations comprises of features essential for securing IoT devices against malware attacks. We have demonstrated this proof of concept
by performing experimental analysis on Snapdragon 820 mobile processor, hosting Android operating system (OS). We developed
a supervised machine learning model for application classification and malware identification by extracting features from the DVFS
states time-series. The experimental results show >0.88 F1-score in classifying benign and malware applications, when evaluated across different
DVFS governors.


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Fig1_v4-1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ 'assets/img/roc_benign_vs_malware.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The figure on the left shows the proposed Machine Learning based detector that uses DVFS signatures. On the right, the ROC curves are shown for classification of a workload into a benign or a malicious application.
</div>

For a detailed report of the work, please refer to our [paper](https://ieeexplore.ieee.org/document/9186163).
