# Positive and negative phases of Boltzmann learning

↑ **Parent:** [Boltzmann machine](boltzmann-machine.md)

Split the units into [visible units](visible-unit.md) $v$, whose patterns occur in the [training data](training-data.md), and [hidden units](hidden-unit.md) $z$. Let $q(v)$ be the empirical [probability distribution](probability-distribution-split.md) and maximize the average [log-likelihood](log-likelihood.md) $\ell=\sum_vq(v)\log p_\beta(v)$, where $p_\beta(v)=\sum_zp_\beta(v,z)$. The positive phase clamps $v$ to data and averages over $q(v)p_\beta(z\mid v)$; the negative phase releases all units and averages over $p_\beta(v,z)$. The displayed difference uses these two [expectations](expected-value-split.md). When both units are visible, the positive pair product is supplied directly by the data.

For a proof, write $\log p_\beta(v)=\log\sum_z e^{-\beta E(v,z)}-\log Z$. Differentiating each finite sum gives, respectively, $-\beta\langle\partial E\rangle_{z\mid v}$ and $-\beta\langle\partial E\rangle_{v,z}$. Since $\partial E/\partial w_{ij}=-x_ix_j$, subtraction proves the rule. Similarly $\partial_{\theta_i}\ell=-\beta(\langle x_i\rangle_+-\langle x_i\rangle_-)$. A small positive step along these [gradients](gradient.md) increases [log-likelihood](log-likelihood.md). The negative term suppresses associations overproduced by the model; strengthening observed pairs alone misses this correction. The identity requires equilibrium [expectations](expected-value-split.md); estimates from insufficiently mixed sampling can give a biased update.

**Table of contents**

- [Visible unit](visible-unit.md)

## ↑ Ancestors (9)

1. [Boltzmann machine](boltzmann-machine.md)
2. [Neural network](neural-network.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
