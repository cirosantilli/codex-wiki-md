# Observed and latent mixture labels

↑ **Parent:** [Finite mixture model](finite-mixture-model.md)

In a [finite mixture model](finite-mixture-model.md) with hidden membership, the component label $Z_i$ is a [latent variable](latent-variable-split.md) and $x_i$ is observed. If an actual recorded label $z_i$ specifies which [mixture component](mixture-component.md) generated $x_i$, then $(x_i,z_i)$ is observed and its [likelihood](likelihood-function.md) contribution is $\pi_{z_i}f_{z_i}(x_i)$. With the label hidden, the observed [likelihood](likelihood-function.md) contribution is the sum $\sum_j\pi_jf_j(x_i)$. A hard assignment chosen from [mixture responsibilities](mixture-responsibility.md) is an inference under the [statistical model](statistical-model-split.md), not an additional recorded label.

## ↑ Ancestors (8)

1. [Finite mixture model](finite-mixture-model.md)
2. [Mixture model](mixture-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
