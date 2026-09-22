<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The squared $L^2(\pi)$ distance has the diagonal identity

$$
\left\lVert\frac{P^t(x,\mathord\cdot)}{\pi(\mathord\cdot)}-1\right\rVert_{2,\pi}^2
=\frac{P^{2t}(x,x)-\pi(x)}{\pi(x)}.
$$

The diagonal excess is nonnegative and decreases with time. Therefore

$$
(2t+1)\{P^{2t}(x,x)-\pi(x)\}
\leq\sum_{k=0}^\infty\{P^k(x,x)-\pi(x)\}.
$$

Using the identity supplied in the question gives

$$
\left\lVert\frac{P^t(x,\mathord\cdot)}{\pi(\mathord\cdot)}-1\right\rVert_{2,\pi}^2
\leq\frac{\mathbb E_\pi\tau_x}{2t+1}.
$$

At $t=8\mathbb E_\pi\tau_x$ the right side is at most $1/16$, up to the immaterial integer rounding. Thus

$$
\boxed{t_{\mathrm{mix}}^{(2)}(x,1/4)\leq8\mathbb E_\pi\tau_x}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
