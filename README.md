# Hybrid-Explore-NMT
This is an implementation of easy-first exploration in BOW search space with only seq2seq+att model. 

As my colleague Lemao Liu mentioned, the first-pass second-pass decoding regime is a way to improve n-gram recall at the target side. This could end up as one of the motivation of this work. 

In the initial motivation of this idea, easy-first means to choose a relatively easy order of decoding the target side sequence instead of the right-to-left regime. The benefit of this is that the model can be flexible enough to seek a better decoding order so that to explore global dependence of words in sequence instead of local dependence which looms so large in the right-to-left regime. 

This hypothesis is bold and could degrade the performance. And till now, only experimental proof could validate or invalidate this hypothesis. 

### Experiment Design

I would like to conduct experiment on neural machine translation as well as neural summarization.

The datasets for doing neural machine translation are IWSLT14 de-en and NIST en-zh.