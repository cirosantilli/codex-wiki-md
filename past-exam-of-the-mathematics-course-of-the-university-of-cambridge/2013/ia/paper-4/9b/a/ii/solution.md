<h1 id="9b/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [circular orbits in an exponential central potential](../../../../../../../circular-orbits-in-an-exponential-central-potential.md), a constant positive radius requires $V_{\rm eff}'(r)=0$, or

$$
l^2=r^3e^{-r}.
$$

Let $h(r)=r^3e^{-r}$. Its derivative is $h'(r)=r^2e^{-r}(3-r)$: it rises from zero to $h(3)=27/e^3$, then falls back to zero. Hence

$$
\boxed{0<l^2<27/e^3\quad\Longrightarrow\quad
0<r_1<3<r_2.}
$$

The strict lower bound matters: the printed upper bound also allows $l=0$, but then there is no finite-radius [circular orbit](../../../../../../../circular-orbit.md). Nonzero [angular momentum](../../../../../../../angular-momentum.md) is an implicit hypothesis of the two-orbit claim.

At a [circular orbit](../../../../../../../circular-orbit.md), use $l^2=r^3e^{-r}$ to obtain

$$
V_{\rm eff}''(r)=-e^{-r}+\frac{3l^2}{r^4}
=e^{-r}\left(\frac3r-1\right).
$$

A small radial displacement $\eta$ satisfies $\ddot\eta=-V_{\rm eff}''(r)\eta$. Therefore **the inner [circular orbit](../../../../../../../circular-orbit.md) is radially stable at fixed [angular momentum](../../../../../../../angular-momentum.md), while the outer orbit is unstable**. The inner perturbation oscillates with squared frequency $e^{-r_1}(3/r_1-1)$; the outer perturbation has an exponentially growing solution. At the limiting value $l^2=27/e^3$, the radii coalesce at $r=3$ and the linear restoring coefficient vanishes.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [9B](../../../9b.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ia](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
