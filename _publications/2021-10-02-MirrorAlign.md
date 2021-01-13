---
title: "Unsupervised Word Alignment via Cross-lingual Contrastive Learning"
collection: publications
permalink: /publication/2021-10-02
venue: 'UNDER REVIEW'
---
[paper](-)
[code](-)

---
*ABSTRACT*

Word alignment is essential for the down-streaming cross-lingual language understanding and generation tasks. 
Recently, the performance of the neural word alignment models~\citep{zenkel2020end,garg2019jointly,koehn2019saliency} 
has exceeded that of statistical models. However, they heavily rely on sophisticated translation models. In this study, 
we propose a super lightweight unsupervised word alignment model, dubbed \textsc{MirrorAlign}, in which a bidirectional 
symmetric attention trained with a contrastive learning objective is introduced, and an agreement loss is employed to 
bind the attention maps, such that the alignments follow mirror-like symmetry hypothesis. Experimental results on 
several public benchmarks demonstrate that our model achieves competitive, if not better, performance compared to the 
state of the art in word alignment while significantly reducing the training and decoding time on average. Further 
ablation analysis and case studies show the superiority of our proposed MirrorAlign. Notably, we recognize our model as 
a pioneer attempt to unify bilingual word embedding and word alignments. Encouragingly, our approach achieves 
16.4$\times$ \textit{speedup} against GIZA++, and 50$\times$ \textit{parameter compression} compared with the 
Transformer-based alignment methods. 

