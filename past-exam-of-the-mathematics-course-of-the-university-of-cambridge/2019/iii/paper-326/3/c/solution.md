<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the interior-domain definition of [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md), so there is no boundary-extension term at $\pm1$. For any admissible scalar [test function](../../../../../../test-function.md) $\varphi$,

$$
\int_{-1}^1u_R(x)\varphi'(x)\,dx
=\int_{-R}^R\varphi'(x)\,dx
=\varphi(R)-\varphi(-R)\leq2.
$$

Thus $\operatorname{TV}(u_R)\leq2$.

Choose $0<\varepsilon<\min\{R,1-R\}$. From the supplied [smooth bump function](../../../../../../smooth-bump-function.md), define

$$
\varphi(x)=e\,\omega_\varepsilon(x-R)-e\,\omega_\varepsilon(x+R).
$$

The two supports are disjoint and inside $(-1,1)$. Each bump has maximum $e^{-1}$, so $\|\varphi\|_\infty\leq1$, while $\varphi(R)=1$ and $\varphi(-R)=-1$. This attains the upper bound, proving

$$
\boxed{\operatorname{TV}(u_R)=2.}
$$

Equivalently, its [distributional derivative](../../../../../../distributional-derivative.md) is $Du_R=\delta_{-R}-\delta_R$, with total variation two. This is [total variation of an interval indicator](../../../../../../total-variation-of-an-interval-indicator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
