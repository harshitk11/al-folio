---
layout: page
title: Logic Encryption
description: Efficient Key-gate Placement And Dynamic Scan Obfuscation Towards Robust Logic Encryption
img: assets/img/logic_cone_attack.PNG
importance: 4
---
Modern ICs consist of different functional modules, called IP cores, provided by different IP vendors located worldwide.
Such a global scale of the semiconductor supply chain eases the development of complex ICs. However, it introduces several
security vulnerabilities like IP-piracy and IC-counterfeiting. Due to the high cost of setting up and maintaining
foundries, fabless companies fabricate their designs using the offshore foundries. A rogue agent in an untrustworthy
foundry can reverse engineer the GDS-II file to extract the functionality of the design. The reverse engineered design
can be overproduced, sold to a rival organization, or may be used to insert Trojans.

Logic encryption has emerged to be a potential solution to the problem of Intellectual Property (IP)-Piracy and
counterfeiting. In this paper, we propose a new logic encryption scheme which dynamically obfuscates the scan operation for
an unauthorized attempt of scan access. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ 'assets/img/proposed_encryption.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Proposed encryption of the Design-for-Test infrastructure.
</div>

A detailed security analysis on the proposed secure DfT infrastructure demonstrates its ability
to thwart SAT attack without compromising the testability of the design. A methodical key-gate placement strategy enables the
proposed scheme to eliminate the leakage of key information through weak key-gate locations, offering protection against path
sensitization and logic cone based attacks. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ 'assets/img/design_flow.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The entire design and test flow of the proposed scheme.
</div>
For a detailed report of the work, please refer to our [paper](https://ieeexplore.ieee.org/document/8946748).
