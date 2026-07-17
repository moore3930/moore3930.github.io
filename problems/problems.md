> "I would rather have questions that can't be answered than answers that can't be questioned." 
>
> -- <cite>Richard Feynman</cite>
>
>

__1. About Shared Vocabulary__

For NLP systems, tokenization is usually the first step. To overcome the so-called "OOV" problem,
BPE was proposed. The core idea behind BPE is merely to compress data, yet its benefits go beyond
handling OOV (after all, nothing beats character-level tokenization for OOV). In some multilingual
scenarios, such as multilingual machine translation, however, things may change. Suppose a system is
trained on extremely imbalanced multilingual data: a language-agnostic tokenizer like BPE allocates
most of the vocabulary to high-resource languages, while splitting low-resource ones into character
sequences. This is tolerable when methods such as temperature sampling are applied — but is it really
an elegant solution? I have been thinking about this from the perspective of information transport,
trying to answer: what is a good way to measure the quality of a vocabulary in multilingual scenarios,
and how to build one?

__2. Quantify Knowledge Transfer__

For multilingual/multi-task systems, we generally rely on specific designs — shared vocabulary, a
shared backbone, or other priors — to encourage knowledge transfer across languages/tasks. We hope
such transfer emerges naturally from our intuition-driven modeling (and it does). I aim to quantify
the degree of transfer or interplay, and further, to measure and encourage such interactions
explicitly.
