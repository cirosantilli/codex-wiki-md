<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $X_s=W_s-as$ and $M_t=\sup_{0\leq s\leq t}X_s$. Split the crossing event according to its endpoint:

$$
\mathbb P(M_t>b)
=\mathbb P(X_t>b)
+\mathbb P(M_t>b,X_t\leq b).
$$

Under the [Cameron-Martin theorem for a linear drift](../../../../../../cameron-martin-theorem-for-a-linear-drift.md), the law of $X$ relative to standard Wiener measure has endpoint density

$$
\exp\!\left(-aW_t-\frac12a^2t\right).
$$

On paths that cross $b$ and end at $x\leq b$, the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) reflects the path after its first hit of $b$ and changes the endpoint to $2b-x\geq b$. Under this reflection the density becomes

$$
e^{-2ab}
\exp\!\left(aW_t-\frac12a^2t\right).
$$

The remaining exponential is the Cameron--Martin density for drift $+a$. Therefore

$$
\mathbb P(M_t>b,X_t\leq b)
=e^{-2ab}\mathbb P(W_t+at\geq b)
=e^{-2ab}\mathbb P(W_t-at\leq-b),
$$

where the last equality uses the symmetry of the [normal distribution](../../../../../../normal-distribution.md). Subtracting the crossing probability from one gives

$$
\boxed{
\mathbb P\!\left(\sup_{0\leq s\leq t}(W_s-as)\leq b\right)
=\mathbb P(W_t-at\leq b)
-e^{-2ab}\mathbb P(W_t-at\leq-b).}
$$

Equivalently, in terms of the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md),

$$
\boxed{
\Phi\!\left(\frac{b+at}{\sqrt t}\right)
-e^{-2ab}\Phi\!\left(\frac{at-b}{\sqrt t}\right).}
$$

This is the [finite-horizon maximum of Brownian motion with negative drift](../../../../../../finite-horizon-maximum-of-brownian-motion-with-negative-drift.md) formula.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
