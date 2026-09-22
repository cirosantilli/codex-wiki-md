# Sigmoid-softmax network gradients

↑ **Parent:** [Backpropagation](backpropagation.md)

For hidden activations $h_j=\sigma(b_j+\sum_rW_{jr}x_r)$ and class probabilities $p_c=\operatorname{softmax}_c(a+Vh)$, a one-hot label $t$ has [log-likelihood](log-likelihood.md) $\ell=\sum_ct_c\log p_c$. Put $\delta_c=t_c-p_c$ and $\Delta_j=h_j(1-h_j)\sum_cV_{cj}\delta_c$. Then

$$
\partial_{a_c}\ell=\delta_c,\quad\partial_{V_{cj}}\ell=\delta_ch_j,\quad\partial_{b_j}\ell=\Delta_j,\quad\partial_{W_{jr}}\ell=\Delta_jx_r.
$$

These follow from the [chain rule](chain-rule.md) and give single-observation [stochastic gradient descent](stochastic-gradient-descent.md) updates for the negative [log-likelihood](log-likelihood.md).

## ↑ Ancestors (10)

1. [Backpropagation](backpropagation.md)
2. [Feedforward neural network](feedforward-neural-network.md)
3. [Neural network](neural-network.md)
4. [Statistical learning](statistical-learning-split.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/3/d/solution.md)
