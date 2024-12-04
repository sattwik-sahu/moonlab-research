---
tags:
  - resources/reading
  - resources/deep-learning
---
> [!help] Resources
> - [Arxiv Insights, *Variational Autoencoders*](https://www.youtube.com/watch?v=9zKuYvjFFS8)
> - [Deepia, *Variational Autoencoders*](https://www.youtube.com/watch?v=qJeaCHQ1k2w)

# What is an Autoencoder?

- Machine that learns a *compression* and *decompression* function.
- Encoder unit compresses the data.
- Bottleneck at the end of encoder outputs the latent space representation of the input.
- Decoder decompresses the latent space representation to original input.

# Variational?

- Machine that learns the parameters of the distribution of the input space.
- Output of encoder is the mean $\mu$ and standard deviation $\sigma$ of the input distribution.
- *Catches the "variation" in the data*.
