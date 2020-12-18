---
layout: page
title: BiasP
description: A DVFS based Exploit to Undermine Resource Allocation Fairness in Linux Platform
img: /assets/img/state_diagram.png
importance: 1
---
In this work, we use the Dynamic Voltage and Frequency Scaling (DVFS) framework of the power management infrastructure in modern SoCs to undermine the resource allocation fairness. DVFS aims to find the right balance between performance and power consumption. It reduces the power consumption of a computing device by scaling down the voltage and frequency based on the targetted performance requirements
of the task. As shown in the following figure, the DVFS states of a commercial Android smartphone is modulated on the basis of its CPU utilization.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/schedutil1.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    CPU utilization of a particular workload and its corresponding allocated DVFS state.
</div>

We formulate a robust task detection methodology, on commercial Linux-kernel based platforms, which is capable of accurately detecting targeted-tasks executing instructions on the CPU-core. We then modify the DVFS attributes to restrict CPU resource allocation to a set of targeted tasks degrading their performance. 


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/target_detect2.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/retinstruction_degradation1.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    On the left, we demonstrate the exploit in a commercial Android smartphone. When a targetted task is actively executing instructions on the CPU-core, BiasP lowers the DVFS state to its lowest value. The corresponding performance degradation for the applications that we had considered, as observed by the decrease in the number of retired instructions, is shown in the figure on the right. 
</div>

For a detailed report of the work, please refer to our [paper](https://dl.acm.org/doi/abs/10.1145/3370748.3406549).
