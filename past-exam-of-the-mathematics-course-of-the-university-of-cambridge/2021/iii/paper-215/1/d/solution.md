<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $T=t_{\mathrm{mix}}^{(2)}(a,1/4)$ and $m=\lceil t_{\mathrm{rel}}\rceil$. The expected local time is

$$
\mathbb E_a\sum_{k=0}^{T-1}\mathbf1_{\{X_k=a\}}
=T\pi(a)+\sum_{k=0}^{T-1}\{P^k(a,a)-\pi(a)\}.
$$

Part c and the supplied return identity give

$$
T\pi(a)\leq8\pi(a)\mathbb E_\pi\tau_a
=8\sum_{k=0}^\infty\{P^k(a,a)-\pi(a)\}.
$$

The second term is bounded by the same infinite sum. Part b now yields

$$
\mathbb E_a\sum_{k=0}^{T-1}\mathbf1_{\{X_k=a\}}
\leq\frac{9e}{e-1}
\sum_{k=0}^m\{P^k(a,a)-\pi(a)\}
\leq\frac{9e}{e-1}\mathbb E_a\sum_{k=0}^m\mathbf1_{\{X_k=a\}}.
$$

**Thus the hinted universal constant $C=9e/(e-1)$ works.**

## ↑ Ancestors (11)

1. [D](../d.md)
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
