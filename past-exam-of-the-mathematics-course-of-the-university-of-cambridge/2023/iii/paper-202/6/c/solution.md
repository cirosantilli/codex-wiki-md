<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each $x$, the bounded local martingale $u(x+B_t)$ is a true martingale. Taking expectations gives

$$
u(x)=\mathbb E[u(x+B_t)]
=\int_{\mathbb R^2}u(x+z)
\frac{e^{-|z|^2/(2t)}}{2\pi t}\,dz
$$

for every $t>0$. Thus $u$ equals its convolution with every [heat kernel](../../../../../../heat-kernel.md). The convolution is smooth, so the originally Borel function $u$ is smooth. Differentiating the [heat semigroup](../../../../../../heat-semigroup.md) identity at $t=0$ gives $\Delta u=0$, so $u$ is a bounded [harmonic function](../../../../../../harmonic-function.md) on the plane. The [harmonic Liouville theorem](../../../../../../harmonic-liouville-theorem.md) now implies that $u$ is constant.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
