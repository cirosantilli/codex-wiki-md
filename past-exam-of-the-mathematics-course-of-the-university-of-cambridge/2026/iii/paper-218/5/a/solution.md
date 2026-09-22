<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For standardized $x\in\mathbb R^8$, model1 computes

$$
h_1=\operatorname{ReLU}(W_1x+b_1)\in\mathbb R^{24},
\quad
h_2=\operatorname{ReLU}(W_2h_1+b_2)\in\mathbb R^{16},
$$

followed by logits $z=W_3h_2+b_3\in\mathbb R^2$ and [softmax function](../../../../../../softmax-function.md) probabilities

$$
p_k(x)=\frac{e^{z_k}}{e^{z_1}+e^{z_2}}.
$$

The parameter count is

$$
(8\cdot24+24)+(24\cdot16+16)+(16\cdot2+2)=650.
$$

For one-hot labels $y_{ik}$, the [categorical cross-entropy loss](../../../../../../categorical-cross-entropy-loss.md) is

$$
-\sum_i\sum_{k=1}^2y_{ik}\log p_k(x_i).
$$

This is the negative conditional log-likelihood of independent categorical labels, equivalently Bernoulli labels in the two-class case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
