> "I would rather have questions that can't be answered than answers that can't be questioned." 
>
> -- <cite>Richard Feynman</cite>
>
>

1. For NLP systems, tokenization is usually the first step. To overcome so-called "OOV" problem,
BPE is proposed. The benefit of BPE is more than handling OOV (afterall, nothing
is better than character-level tokenization for OOV), however the main idea behind BPE is 
to compress data. In some multilingual senarios, such as multilingual machine translation,
thing may change. Suppose that a system is trained on extremely imbalanced multilingual 
datasets, language-agnostic tokenizer, like BPE, will place most of the vocabulary space to
high-resource data, and split low-resource data into a sequence of characters. From the perspective
of data compression, it is still fine. BUT, does it a really good choice? I am thinking about 
this issue from the angle of information transport, and try to answer, what is a good way to measure the 
quality of a vocabulary in cross-lingual senarios and how to build it?

