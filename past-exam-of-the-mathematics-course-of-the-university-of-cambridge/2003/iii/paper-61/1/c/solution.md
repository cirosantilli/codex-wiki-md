<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The other roots of $w(\nu)=w(k)$ satisfy

$$
\nu^2+k\nu+k^2+1=0,\qquad
\nu_\pm=\frac{-k\pm\sqrt{-3k^2-4}}2.
$$

For $k\in D_+$, select the unique other root $\nu(k)$ with negative imaginary part. This is a [dispersion symmetry elimination of a boundary trace](../../../../../../dispersion-symmetry-elimination-of-a-boundary-trace.md), but only the root in the spatial-transform half-plane may be used. The root is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) throughout $D_+$: the upper branch point $2i/\sqrt3$ lies above its boundary. Near the real axis one other root is above and one below; a root can cross the real axis only when $\operatorname{Re}w=0$, so the lower-root choice persists throughout $D_+$.

Evaluate the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) at $\nu$, using the same time transforms because $w(\nu)=w(k)$:

$$
G_2=Q_0(\nu)+(1+\nu^2)G_0-i\nu G_1-e^{wT}\widehat q(\nu,T).
$$

Consequently

$$
F(k,T)=H(k,T)+e^{w(k)T}\widehat q(\nu(k),T),
$$

where the completely known spectral density is

$$
\boxed{H(k,T)=-Q_0(\nu(k))+(k^2-\nu(k)^2)G_0(k,T)-i(k-\nu(k))G_1(k,T).}
$$

The remaining term in the solution formula has integral

$$
\int_{\partial D_+}e^{ikx+w(k)(T-t)}\widehat q(\nu(k),T)\,dk=0.
$$

Its transformed argument stays in the lower half-plane, it is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) inside $D_+$, and $e^{w(T-t)}$ does not grow there. Spatial exponential decay closes the truncated domain. Thus the formula in part (b), with $F$ replaced by $H$, uses only the prescribed initial value and the two prescribed boundary traces. It contains no unknown $g_2$ or final-time solution transform. Keeping the inadmissible upper root instead would invalidate this elimination.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
