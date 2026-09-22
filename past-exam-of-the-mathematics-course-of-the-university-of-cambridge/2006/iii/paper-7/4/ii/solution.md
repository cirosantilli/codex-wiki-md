<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $L=2\pi$ and represent the [circle](../../../../../../circle.md) by $[0,L)$. The full [orthonormal basis](../../../../../../orthonormal-basis.md) of [Haar wavelets](../../../../../../haar-wavelet.md) includes the constant $H_*=L^{-1/2}$ and, for every dyadic interval $I$ of length $\ell=L2^{-j}$, the normalized detail

$$
H_I=\ell^{-1/2}(\mathbf1_{I_{\mathrm{left}}}-\mathbf1_{I_{\mathrm{right}}}),\qquad c_I=\int_0^Lf(t)\overline{H_I(t)}\,dt.
$$

Take half-open intervals and the corresponding values at their boundaries, so every point belongs to exactly one interval at each level. The constant basis function is necessary: if it were omitted, even $f\equiv1$ could not satisfy the asserted convergence. We use the full conventional [Haar wavelet](../../../../../../haar-wavelet.md) system in the threshold sum.

Let $A_Jf$ be the function equal to the mean of $f$ on each level-$J$ dyadic interval. Comparing the means on a parent and its two children proves the [Haar refinement identity](../../../../../../haar-refinement-identity.md) directly: the difference between the child mean and the parent mean is the appropriate value of $c_IH_I$. Inductively this gives the [Haar projection](../../../../../../haar-projection.md)

$$
A_Jf=c_*H_*+\sum_{j=0}^{J-1}\sum_{I\text{ at level }j}c_IH_I,\qquad c_*H_*=\frac1L\int_0^Lf(t)\,dt.
$$

Writing $\omega_f(s)=\sup_{\operatorname{dist}(x,y)\leq s}|f(x)-f(y)|$ for the [modulus of continuity](../../../../../../modulus-of-continuity.md), the cell-average formula yields

$$
\|A_Jf-f\|_\infty\leq\omega_f(L2^{-J})\longrightarrow0.
$$

For a detail on a cell $I$, its integral is zero. Subtracting $f(x_I)$ for any $x_I\in I$ therefore gives the coefficient estimate

$$
|c_I|\leq\int_I|f(t)-f(x_I)||H_I(t)|\,dt\leq\omega_f(\ell)\sqrt\ell.
$$

In particular $|c_I|\leq2\|f\|_\infty\sqrt\ell$, so for every $\delta>0$ only finitely many details can have $|c_I|\geq\delta$. The hard-threshold sum

$$
T_\delta f=\sum_{|c_H|\geq\delta}c_HH
$$

is thus a well-defined finite sum. Its chosen details need not form a complete set of levels; this is why convergence of the [Haar projections](../../../../../../haar-projection.md) alone does not prove the result.

Fix $\eta>0$. Choose $J\geq1$ so that $\omega_f(L2^{-J})\leq\eta$. All finer details satisfy $|c_I|\leq\eta\sqrt L\,2^{-j/2}$ at level $j\geq J$. For sufficiently small $\delta$, every nonzero coefficient at levels below $J$, and the constant coefficient if nonzero, is retained. Also choose the unique integer $K\geq J$ such that

$$
\frac{\delta2^{K/2}}{\sqrt L}\leq\eta<\frac{\delta2^{(K+1)/2}}{\sqrt L}.
$$

For $j>K$ we have $|c_I|\leq\eta\sqrt L2^{-j/2}<\delta$, so no such detail is retained. Consequently $T_\delta f$ differs from $A_{K+1}f$ only by omitted details at levels $J$ through $K$. At any point there is at most one supported detail per level, and an omitted detail has magnitude at most $\delta/\sqrt{L2^{-j}}$. The [geometric bound for omitted Haar details](../../../../../../geometric-bound-for-omitted-haar-details.md) gives

$$
\|T_\delta f-A_{K+1}f\|_\infty\leq\sum_{j=J}^K\frac{\delta2^{j/2}}{\sqrt L}\leq\frac{\eta}{1-2^{-1/2}}.
$$

Since $\|A_{K+1}f-f\|_\infty\leq\eta$, we conclude

$$
\|T_\delta f-f\|_\infty\leq\left(1+\frac1{1-2^{-1/2}}\right)\eta.
$$

The right side can be made arbitrarily small, proving [uniform hard-threshold convergence of normalized Haar expansions](../../../../../../uniform-hard-threshold-convergence-of-normalized-haar-expansions.md):

$$
\boxed{\left\|\sum_{|\widehat f(H)|\geq\delta}\widehat f(H)H-f\right\|_\infty\longrightarrow0\quad(\delta\downarrow0).}
$$

The square-root scaling imposed by the specified $L^2$ normalization is what makes the omitted contributions a controlled [geometric series](../../../../../../geometric-series.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
