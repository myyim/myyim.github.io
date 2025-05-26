## Correlations in weights in pretrained small language models

### Abstract

Motivation:
1. Multiple studies reported that pruning certain layers, or even entire blocks, in a pretrained LLM has a minimal impact on its performance, suggesting redundancy within their model architectures.
2. Could we identify the redundancy within their model architectures by looking into the weights?
3. Could we develop a smaller language model with comparable performance of a larger model by removing the redundancy?
4. Could we understand the values of the weights better?

Methods:


Observations:

Plans:
1. Study how the correlation structures evolve during training by looking into different checkpoints
2. Examine the changes of the correlation structures upon fine-tuning
3. Explore the functional significance of layers and attention heads with different correlations by pruning techniques
4. Investigate the correlation structures in larger language models

---
My notes

<img src="note1.jpg" height="130" /><img src="note2.jpg" height="130" /><img src="note3.jpg" height="130" />

The derivation can be found [here](yim_derivation_LIF.pdf).
