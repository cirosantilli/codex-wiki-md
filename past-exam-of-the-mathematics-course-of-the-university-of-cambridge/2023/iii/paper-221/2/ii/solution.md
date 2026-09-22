<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For discrete $X$,

$$
\beta=\sum_xp(x)\pi(x)\mu(x).
$$

Perturbing the marginal mass $p(x)$ contributes $\pi(X)\mu(X)-\beta$. Perturbing $\pi(x)=\mathbb E[A\mid X=x]$ contributes

$$
\mu(X)\{A-\pi(X)\}.
$$

Their sum is $A\mu(X)-\beta$. Finally, the [influence function](../../../../../../influence-function.md) of

$$
\mu(x)=\mathbb E[Y\mid A=0,X=x]
$$

is

$$
\frac{\mathbf1_{\{A=0,X=x\}}}{p(x)\{1-\pi(x)\}}
\{Y-\mu(x)\}.
$$

Multiplication by the derivative $p(x)\pi(x)$ of $\beta$ with respect to $\mu(x)$ and summation over $x$ gives

$$
(1-A)\frac{\pi(X)}{1-\pi(X)}\{Y-\mu(X)\}.
$$

Adding the three contributions yields the claimed mean-zero [influence curve](../../../../../../influence-function.md)

$$
\boxed{(1-A)\frac{\pi(X)}{1-\pi(X)}\{Y-\mu(X)\}
+A\mu(X)-\beta.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
