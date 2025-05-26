## Correlations in weights in pretrained small language models

### Abstract

Motivation:
1. Multiple studies reported that pruning certain layers, or even entire blocks, in a pretrained LLM has a minimal impact on its performance, suggesting redundancy within their model architectures.
2. Could we identify the redundancy within their model architectures by looking into the weights or correlation of weights?
3. Could we better understand the weights in different attention heads, along the layers, in attention and MLP layers?

Theory:
1. The resulting embedding in the attention layer is a function of the product of W_q and W_k, as well as the product of W_o and W_v.
2. The MLP layer has the gated and up projection in parallel and then the two streams are combined with elementwise multiplication and fed into down projection.

Methods:
For each LLM, we computed the followings:
1. 

Observations:

Future plans:
1. Study how the correlation structures evolve during training by looking into different checkpoints
2. Examine the changes of the correlation structures upon fine-tuning
3. Explore the functional significance of layers and attention heads with different correlations by pruning techniques
4. Investigate the correlation structures in larger language models

Results:


---
My notes

<img src="note1.jpg" height="130" /><img src="note2.jpg" height="130" /><img src="note3.jpg" height="130" />

