> "I would rather have questions that can't be answered than answers that can't be questioned." 
>
> -- <cite>Richard Feynman</cite>
>
>

__1. About Shared Vocabulary__

For NLP systems, tokenization is usually the first step. To overcome so-called "OOV" problem,
BPE is proposed. The main idea behind BPE is to compress data only, but the benefit of 
BPE is more than handling OOV (afterall, nothing is better than character-level tokenization
for OOV). However, in some multilingual senarios, such as multilingual machine translation,
thing may change. Suppose that a system is trained on extremely imbalanced multilingual 
datasets, language-agnostic tokenizer, like BPE, will place most of the vocabulary space to
high-resource data, and split low-resource data into a sequence of characters. It is still fine, if temperature 
sampling like methods are applied. BUT, does it a really elegant solution? I am thinking about 
this issue from the angle of information transport, and try to answer, what is a good way to measure the 
quality of a vocabulary in cross-lingual senarios and how to build it?

__2. Quantify Knowledge Transfer__

For multilingual/multi-task systems, generally, we rely on some specific designs to encourage 
knowledge transfer among languages/tasks, like shared vocabulary, backbone or other priors.
We hope transfer occurs naturally following our insight-driven modeling (actually it does). 
I am seeking to quantify the ratio of transfer or interference, moreover, to encourage 
such interactions in an explicit way.