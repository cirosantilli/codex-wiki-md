<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [chain rule](../../../../../../chain-rule.md) to the squared loss, using the same pre-update weights throughout a forward and backward pass. At the output, $\partial E/\partial z_k=z_k-t_k$ and $\partial z_k/\partial x_k=g_k'(x_k)$. Therefore

$$
\frac{\partial E}{\partial w_{jk}}=(z_k-t_k)g_k'(x_k)z_j.
$$

For a [gradient descent](../../../../../../gradient-descent.md) step of size $\eta>0$, define $\delta_k=\eta(t_k-z_k)g_k'(x_k)$. This gives $\boxed{\Delta w_{jk}=\delta_kz_j}$.

A hidden activation affects all output units to which it connects. Thus

$$
\frac{\partial E}{\partial x_j}=g_j'(x_j)\sum_kw_{jk}(z_k-t_k)g_k'(x_k),
$$

and

$$
\boxed{\delta_j=g_j'(x_j)\sum_kw_{jk}\delta_k,\qquad\Delta w_{ij}=\delta_jz_i}.
$$

The learning rate is already contained in $\delta_k$ and hence in $\delta_j$; do not multiply by it a second time. For a [sigmoid function](../../../../../../sigmoid-function.md), $g'(x)=g(x)[1-g(x)]$. Thresholds can be treated as negative biases with an extra constant input and updated by the same derivative rule.

This is [squared-error backpropagation](../../../../../../squared-error-backpropagation.md). The forward pass computes activations, while the backward pass transports output-loss derivatives through the outgoing weights and the derivatives of the [activation functions](../../../../../../activation-function.md), yielding an error signal for every [hidden unit](../../../../../../hidden-unit.md). That reverse flow of derivatives explains the name [backpropagation](../../../../../../backpropagation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
