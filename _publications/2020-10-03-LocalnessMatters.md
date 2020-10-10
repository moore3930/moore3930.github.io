---
title: "SLocalness Matters: The Evolved Cross-Attention for Non-Autoregressive Translation"
collection: publications
permalink: /publication/2020
venue: 'COLING'
---
[paper](https://arxiv.org/pdf/2010.02693.pdf)
[code](https://github.com/moore3930/SlotRefine)

---
*ABSTRACT*
Non-autoregressive translation (NAT) significantly accelerates the inference process via predicting the entire target 
sequence. However, due to the lack of autoregressive factorization, it is difficult for the decoder to adequately 
capture the source contexts. To response this problem, we propose a novel evolved cross-attention for the NAT decoder 
by modeling the local and global attention simultaneously. Experimental results on Romanian$\Rightarrow$English, 
English$\Rightarrow$German and Chinese$\Rightarrow$English translation tasks demonstrate that our approach significantly 
and consistently improves translation quality over strong NAT baselines. Encouragingly, the proposed model outperforms 
its autoregressive counterpart, Transformer. 

