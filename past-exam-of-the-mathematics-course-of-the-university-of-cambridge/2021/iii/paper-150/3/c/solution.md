<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Shrink the constant $c$ from part b if necessary. Put $L=\log|t|$. Zeros in the disk appearing in the supplied partial-fraction formula have $\log|\gamma|=L+O(1/|t|)$, so part b ensures

$$
\beta\leq1-\frac cL
$$

for every such zero.

If $\sigma\geq1+c/(2L)$, absolute convergence of the [logarithmic derivative](../../../../../../logarithmic-derivative.md) gives

$$
\left|\frac{\zeta'(s)}{\zeta(s)}\right|
\leq\sum_{n\geq1}\frac{\Lambda(n)}{n^\sigma}
=-\frac{\zeta'(\sigma)}{\zeta(\sigma)}
\ll\frac1{\sigma-1}\ll L,
$$

with the region $\sigma\geq2$ even easier.

It remains to take $1-c/(2L)<\sigma<1+c/(2L)$. Set

$$
s_0=1+\frac c{2L}+it.
$$

For every local zero, both $\Re(s-\rho)$ and $\Re(s_0-\rho)$ are positive and comparable, while $|s-s_0|\ll1/L$. The partial-fraction formula at $s_0$, together with the preceding Euler-product bound, gives

$$
\sum_\rho\Re\frac1{s_0-\rho}\ll L.
$$

Since $\Re(s_0-\rho)\gg1/L$, it follows that

$$
\sum_\rho\frac1{|s_0-\rho|^2}\ll L^2.
$$

Subtracting the partial-fraction formulas at $s$ and $s_0$ now yields

$$
\left|\frac{\zeta'(s)}{\zeta(s)}-\frac{\zeta'(s_0)}{\zeta(s_0)}\right|
\ll |s-s_0|\sum_\rho\frac1{|s-\rho||s_0-\rho|}+L
\ll L.
$$

Therefore the [logarithmic derivative inside the zeta zero-free region](../../../../../../logarithmic-derivative-inside-the-zeta-zero-free-region.md) satisfies

$$
\boxed{\frac{\zeta'(s)}{\zeta(s)}\ll\log|t|}
$$

throughout the required half-width region.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
