<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the uniform nonzero amplitude be $R$, so $\mu=R^2-\alpha R$ and $B=0$. Write $r=R(2R-\alpha)$. A perturbation with Fourier [wavenumber](../../../../../../wavenumber.md) $k=n\pi/L$ has [stability matrix](../../../../../../stability-matrix.md)

$$
M_k=\begin{pmatrix}-r-k^2&-R\\-2\sigma\delta Rk^2&-\sigma k^2\end{pmatrix},\qquad
\tau_k=-r-(1+\sigma)k^2,\qquad
D_k=\sigma k^2[k^2+r-2\delta R^2].
$$

The constant $B$ mode is disallowed because the conserved mean is prescribed. At $k=0$ the only allowed mode has [eigenvalue](../../../../../../eigenvalue.md) $-r$, so homogeneous stability requires $r>0$. Then every nonzero-mode [trace](../../../../../../matrix-trace.md) is negative, and its [determinant](../../../../../../determinant.md) is smallest in sign at the smallest allowed $k^2$. The exact [periodic stability criterion for a conserved-field uniform amplitude](../../../../../../periodic-stability-criterion-for-a-conserved-field-uniform-amplitude.md) is

$$
\boxed{r>0,\qquad \left(\frac\pi L\right)^2+2(1-\delta)R^2-\alpha R>0.}
$$

A zero in either inequality is a marginal case requiring nonlinear analysis. The zero-amplitude branch, separately, has amplitude growth rates $\mu-k^2$ and nonzero conserved-field growth rates $-\sigma k^2$, and is strictly stable when $\mu<0$.

For the long-domain interpretation one may take $\alpha>0$ by reversing the sign of $A$, and first consider the positive upper branch $R>\alpha/2$. It is homogeneously stable even though sufficiently long spatial modulations grow whenever

$$
2(1-\delta)R^2-\alpha R<0.
$$

For $0<\delta<1$, this gives

$$
\boxed{\frac\alpha2<R<\frac\alpha{2(1-\delta)},\qquad -\frac{\alpha^2}{4}<\mu<\frac{\alpha^2(2\delta-1)}{4(1-\delta)^2}.}
$$

At a fixed finite $L$ the actual unstable part is smaller: it must also satisfy $(\pi/L)^2<\alpha R-2(1-\delta)R^2$. For $\delta\geq1$, the right side is positive for every positive upper-branch $R$, so every such state is unstable to sufficiently long waves. The physical mechanism is feedback from the conserved field: an increase in $A^2$ reduces local $B$, and the term $-AB$ reinforces that increase.

There are two important limits on the wording of the requested stability conclusion. First,

$$
\frac{dR}{d\mu}=\frac1{2R-\alpha}
$$

never vanishes at a finite regular point of this branch. At its fold the [derivative](../../../../../../derivative.md) is infinite. Thus a condition of zero $dR/d\mu$ cannot literally occur here. The meaningful contrast is that **a positive-slope, homogeneously stable branch can still have a growing spatial mode**.

Second, a long-wave conclusion cannot be asserted for every finite periodic domain. For example, $\alpha=1$, $\delta=2$, $\sigma=1$, $R=1$, $\mu=0$, $L=1$ give $r=1$ and $k^2+r-2\delta R^2=n^2\pi^2-3>0$ for every nonzero integer $n$. This state is strictly stable even though $\delta>1$. Nor does the unrestricted statement include every sign of $R$: $\alpha=1$, $\delta=2$, $R=-1/10$, $\mu=11/100$ give $r=3/25$ and $r-2\delta R^2=2/25>0$, hence stability for every period and every $\sigma>0$. These examples distinguish the exact stated real-variable periodic problem from its intended positive-amplitude, long-layer interpretation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
