---
title: "SlotRefine: A Fast Non-Autoregressive Model for Joint Intent Detection and Slot Filling"
collection: publications
permalink: /publication/2020-10-01
venue: 'EMNLP'
---
[paper](https://arxiv.org/pdf/2010.02693.pdf)
[code](https://github.com/moore3930/SlotRefine)

---
Slot filling and intent detection are two main tasks in spoken language understanding (SLU) system. In this paper, 
we propose a novel non-autoregressive model named SlotRefine for joint intent detection and slot filling. Besides, 
we design a novel two-pass iteration mechanism to handle the uncoordinated slots problem caused by conditional 
independence of non-autoregressive model. Experiments demonstrate that our model significantly outperforms previous 
models in slot filling task, while considerably speeding up the decoding (up to $\times$10.77). In-depth analyses show 
that 1) pretraining schemes could further enhance our model; 2) two-pass mechanism indeed remedy the uncoordinated slots.

