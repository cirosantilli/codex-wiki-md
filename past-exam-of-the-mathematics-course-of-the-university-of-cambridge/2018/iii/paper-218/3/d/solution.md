<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For one observation, let $\ell_i=\sum_{c=0}^1t_{ic}\log p_{ic}$ and define $\delta_{ic}=t_{ic}-p_{ic}$. Differentiating the [softmax function](../../../../../../softmax-function.md) and its [log-likelihood](../../../../../../log-likelihood.md) gives $\partial\ell_i/\partial o_{ic}=\delta_{ic}$. The [sigmoid-softmax network gradients](../../../../../../sigmoid-softmax-network-gradients.md) are

$$
\boxed{\frac{\partial\ell_i}{\partial a_c}=\delta_{ic},\qquad\frac{\partial\ell_i}{\partial V_{cj}}=\delta_{ic}h_{ij},}
$$



$$
\Delta_{ij}=h_{ij}(1-h_{ij})\sum_{c=0}^1V_{cj}\delta_{ic},\qquad
\boxed{\frac{\partial\ell_i}{\partial b_j}=\Delta_{ij},\qquad\frac{\partial\ell_i}{\partial W_{jr}}=\Delta_{ij}x_{ir}.}
$$

These equations are [backpropagation](../../../../../../backpropagation.md): use the [chain rule](../../../../../../chain-rule.md) through the output affine map, then $\sigma'(u)=\sigma(u)(1-\sigma(u))$ through the hidden units, then the input affine map.

For a learning rate $\eta>0$, select one observation and update every parameter by $\theta\leftarrow\theta+\eta\nabla\ell_i(\theta)$, computing all entries of the [gradient](../../../../../../gradient.md) from the old parameters before applying the update. A uniformly selected observation gives an unbiased gradient of the average log-likelihood; multiplying by 3000 would instead estimate the gradient of the sum. Equivalently perform [stochastic gradient descent](../../../../../../stochastic-gradient-descent.md) on the negative log-likelihood. Batch size one makes one update per observation, and five epochs make five passes through the data, typically with a fresh random ordering on each pass.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
