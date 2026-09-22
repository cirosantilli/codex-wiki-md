<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $Y=g(X)-\mathbb Eg(X)$ and $H(\lambda)=\log\mathbb Ee^{\lambda Y}$. Apply the assumed Poisson log-Sobolev inequality to $f=e^{\lambda g}$. Since $|Dg|\leq1$ and $|e^a-1|\leq\lambda e^\lambda$ for $|a|\leq\lambda$,

$$
\frac{|D(e^{\lambda g})(x)|^2}{e^{\lambda g(x)}}
=e^{\lambda g(x)}|e^{\lambda Dg(x)}-1|^2
\leq\lambda^2e^{2\lambda}e^{\lambda g(x)}.
$$

After division by $\mathbb Ee^{\lambda g}$, the entropy bound becomes

$$
\lambda H'(\lambda)-H(\lambda)\leq C\lambda^2e^{2\lambda}.
$$

Because $(H(\lambda)/\lambda)'=(\lambda H'-H)/\lambda^2$ and $H'(0)=0$, integration from $0$ to $\lambda$ gives

$$
H(\lambda)\leq\psi(\lambda)
:=\frac{C\lambda}{2}(e^{2\lambda}-1).
$$

The [Chernoff bound](../../../../../../chernoff-bound.md) and optimization over $\lambda\geq0$ therefore yield

$$
\mathbb P(Y\geq t)
\leq\exp\left\{-\sup_{\lambda\geq0}
[\lambda t-\psi(\lambda)]\right\}
=e^{-\psi^*(t)},
$$

where $\psi^*$ is the [Legendre transform of a cumulant-generating function](../../../../../../legendre-transform-of-a-cumulant-generating-function.md), also called the Chernoff-Cramér transform.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
