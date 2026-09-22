<h1 id="a/3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[conditional dominated convergence theorem](../../../../../../conditional-dominated-convergence-theorem.md) states that if $U_n\to U$ almost surely and $|U_n|\leq H$ for an integrable $H$, then

$$
\mathbb E(U_n\mid\mathcal G)\to\mathbb E(U\mid\mathcal G)
\quad\text{almost surely and in }L^1.
$$

For an [indicator function](../../../../../../indicator-function.md) $Z=\mathbf1_B$, $B\in\mathcal G$, the defining integrals of [conditional expectation](../../../../../../conditional-expectation.md) immediately give the take-out identity: testing on $A\in\mathcal G$ replaces $A$ by $A\cap B$. Finite linear combinations give it for simple $\mathcal G$-measurable $Z$. Approximating a bounded such $Z$ by uniformly bounded simple functions and using [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) proves

$$
\mathbb E(ZX\mid\mathcal G)=Z\mathbb E(X\mid\mathcal G)
$$

for bounded $Z$.

For the stated unbounded case, clip $Z$ to $Z_m=(-m)\vee(Z\wedge m)$. Then $XZ_m\to XZ$ and $|XZ_m|\leq|XZ|$, an integrable bound by hypothesis. [conditional dominated convergence theorem](../../../../../../conditional-dominated-convergence-theorem.md) and the bounded identity give

$$
\mathbb E(XZ\mid\mathcal G)
=\lim_m\mathbb E(XZ_m\mid\mathcal G)
=\lim_m Z_m\mathbb E(X\mid\mathcal G)
=\boxed{Z\mathbb E(X\mid\mathcal G)}
$$

almost surely. The equality with the integrable [conditional expectation](../../../../../../conditional-expectation.md) also proves integrability of the final product; it is not necessary to assume that separately.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
