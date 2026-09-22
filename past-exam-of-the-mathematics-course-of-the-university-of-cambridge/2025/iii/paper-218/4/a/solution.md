<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Encode the two classes by the standard basis vectors of $\mathbb R^2$. With [rectified linear unit](../../../../../../rectified-linear-unit.md) $r(t)=\max(t,0)$ applied coordinatewise and [softmax function](../../../../../../softmax-function.md) $s_j(z)=e^{z_j}/\sum_ke^{z_k}$, the fitted [feedforward neural network](../../../../../../feedforward-neural-network.md) is

$$
\widehat p(x)=s\!\left(W_3r\!\left(W_2r(W_1x+b_1)+b_2\right)+b_3\right),
$$

where $W_1\in\mathbb R^{40\times40}$, $b_1\in\mathbb R^{40}$, $W_2\in\mathbb R^{20\times40}$, $b_2\in\mathbb R^{20}$, $W_3\in\mathbb R^{2\times20}$, and $b_3\in\mathbb R^2$. The number of trainable parameters is

$$
\boxed{40\cdot40+40+20\cdot40+20+2\cdot20+2=2502.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
