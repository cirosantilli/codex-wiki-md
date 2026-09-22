<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work initially with $\operatorname{Re}s>1$, where the [nonholomorphic Eisenstein series](../../../../../../nonholomorphic-eisenstein-series.md) and its differentiated series converge locally absolutely. For $\gamma=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)\in SL_2(\mathbb Z)$, the identities

$$
\operatorname{Im}(\gamma\tau)=\frac y{|c\tau+d|^2},\qquad
m\gamma\tau+n=\frac{(ma+nc)\tau+(mb+nd)}{c\tau+d}
$$

show that each summand at $\gamma\tau$ becomes the summand indexed by $(ma+nc,mb+nd)$ at $\tau$. Reindexing the nonzero integer pairs therefore proves

$$
\boxed{G(\gamma\tau,s)=G(\tau,s).}
$$

Here $y^s$ and the denominator powers use logarithms of positive real numbers, so there is no ambiguity for complex $s$.

For the nonnegative [Laplace-Beltrami operator](../../../../../../laplace-beltrami-operator.md) of the [hyperbolic plane](../../../../../../hyperbolic-plane.md), $\Delta y^s=-y^2\partial_y^2y^s=s(1-s)y^s$. If $(m,n)=r(c,d)$ with $(c,d)$ primitive and $r>0$, choose a matrix in $SL_2(\mathbb Z)$ with bottom row $(c,d)$. The corresponding summand is

$$
\frac{y^s}{|m\tau+n|^{2s}}=r^{-2s}\big(\operatorname{Im}(\gamma\tau)\big)^s.
$$

The [Laplace-Beltrami operator](../../../../../../laplace-beltrami-operator.md) commutes with hyperbolic [isometries](../../../../../../isometry.md), so this summand has [eigenvalue](../../../../../../eigenvalue.md) $s(1-s)$. This also covers $m=0$, or follows there directly. Termwise differentiation now gives

$$
\boxed{\Delta G(\tau,s)=s(1-s)G(\tau,s).}
$$

The equation describes an automorphic eigenfunction; it does not assert that this noncuspidal function belongs to the square-integrable discrete [spectrum](../../../../../../spectrum-functional-analysis.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
