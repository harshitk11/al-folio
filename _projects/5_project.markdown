---
layout: page
title: EM based Malware Analysis
description: Machine Learning in Wavelet Domain for Electromagnetic Emission based Malware Analysis
img: /assets/img/EM-overview.PNG
importance: 2
---
In this work, we present a signal processing and machine learning (ML) based methodology to leverage Electromagnetic (EM) emissions from an embedded device to remotely detect a malicions application running on the device and classify the malicious application into a malware family. The experimental demonstration on Open-Q 820 development platform demonstrates 0.99 F1 schore in detecting malware and 0.88 F1 score in uniquely classifying malwares among 8 different malware families using Support Vector Machines and Random Fores ML models.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/EM-overview.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    EM side-channel monitoring setup, feature extractor, and ML model for detecting threat and classifying its characteristic behavior.
</div>

We demonstrate unique data-processing methods by coupling 1D-STFR and 2D-DWT on the spectrogram of EM side-channel traces.


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/benign-vs-malware-f1.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/malware-family-em.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    [left] Validation Score for malware detection, [right] Validation score for classifying a malicious workload into malware families.
</div>

For a detailed report of the work, please refer to our [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9432941).
