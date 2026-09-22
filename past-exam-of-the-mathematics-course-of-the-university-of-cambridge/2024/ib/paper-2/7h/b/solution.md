<h1 id="7h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now $d=1/e$, and both constraints are active. Therefore

$$
x_2=\frac1{e^2},
\qquad
x_1=c-x_2=\frac2{e^2}.
$$

The first stationarity equation gives

$$
\lambda=1-\log2>0,
$$

and the second gives

$$
\mu=\frac{2\log2}{e}>0.
$$

Thus all multiplier and complementary-slackness conditions hold, and

$$
\boxed{x_1=\frac2{e^2},
\qquad
x_2=\frac1{e^2}},
$$

with minimum value

$$
\boxed{\frac{2\log2-5}{e^2}}.
$$

The observation is that lowering $d$ activates the second constraint and moves the optimum to the intersection of the two active boundaries. Rewriting $\sqrt{x_2}\leq d$ as $x_2\leq d^2$ shows that the feasible set is convex, while $x_1\log x_1-x_2$ is convex. Hence the [active-set transition in capped resource allocation](../../../../../../active-set-transition-in-capped-resource-allocation.md) and the KKT candidates above give the unique global minima, not merely local stationary points.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7H](../../7h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
