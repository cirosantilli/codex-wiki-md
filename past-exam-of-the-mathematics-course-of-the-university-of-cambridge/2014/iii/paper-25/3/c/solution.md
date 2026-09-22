<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $L=\log t$ and $\ell=\log L$, for sufficiently large $t$. Apply the [Landau zero-free-region theorem](../../../../../../landau-zero-free-region-theorem.md) with

$$
\eta=a(\ell/L)^{2/3},
$$

where $a>0$ is fixed and small enough that $\eta\le1/4$. On its two discs, the real part is at least $1-3\eta/4$ and the imaginary part is comparable to $t$. The given [Richert bound for the Riemann zeta function](../../../../../../richert-bound-for-the-riemann-zeta-function.md) therefore gives, on the part left of one,

$$
\log|\zeta(z)|\le C'\eta^{3/2}L+\tfrac23\log L+O(1)=O(\ell).
$$

On the part right of one, the separately given $O(\log^{2/3}t)$ bound gives the same conclusion. We may thus choose $M=L^A$ for one fixed sufficiently large $A$. Also $\log(1/\eta)=O(\ell)$, so the logarithmic term in the [Landau zero-free-region theorem](../../../../../../landau-zero-free-region-theorem.md) is $O(\ell)$. Its conclusion is

$$
\boxed{\zeta(\sigma+it)\ne0\quad\text{for}\quad\sigma\ge1-\frac c{(\log t)^{2/3}(\log\log t)^{1/3}}}
$$

for large $t$ and a sufficiently small positive $c$. [Complex conjugation](../../../../../../complex-conjugation.md) supplies negative heights. This is the [Vinogradov-Korobov zero-free region](../../../../../../vinogradov-korobov-zero-free-region.md). Only the stated Richert upper bounds, the [Euler product](../../../../../../euler-product.md), the [pole](../../../../../../pole.md) at one and the proved [Landau zero-free-region theorem](../../../../../../landau-zero-free-region-theorem.md) were used; no prior zero-free-region theorem was assumed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
