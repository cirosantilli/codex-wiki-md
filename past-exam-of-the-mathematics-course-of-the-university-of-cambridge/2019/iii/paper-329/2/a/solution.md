<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $b=\Delta\rho\,g>0$, so $p_{\rm ext}=bh$. Balancing the viscous and pressure terms in the [axisymmetric viscous-sheet stretching equations](../../../../../../axisymmetric-viscous-sheet-stretching-equations.md), together with fixed [volume](../../../../../../volume.md), suggests a [similarity solution](../../../../../../similarity-solution.md)

$$
h=t^{-1}H(\eta),\qquad u=t^{-1/2}U(\eta),\qquad \eta=r/\sqrt t.
$$

The [conservation of mass](../../../../../../mass-conservation.md) equation becomes

$$
-H-\frac\eta2H'+\frac1\eta(\eta HU)'=0,
\qquad [\eta H(U-\eta/2)]'=0.
$$

There is no ongoing source at the origin, so the integration constant vanishes and $U=\eta/2$ wherever $H>0$. Thus $u=r/(2t)$. Substitution into radial [force balance](../../../../../../force-balance.md) gives

$$
\left(\frac{3\mu}{t}-bh\right)h_r=0,
\qquad (3\mu-bH)H'=0.
$$

A differentiable $H$ cannot have nonzero derivative on an interval while being fixed there at $3\mu/b$. Hence $H'=0$: the spreading sheet has uniform thickness.

At the material edge, $R'=u(R,t)=R/(2t)$. Since $\sigma_{rr}=-bh+3\mu/t$, the edge condition $h\sigma_{rr}=-bh^2/2$ fixes $h=6\mu/(bt)$. Fixed [volume](../../../../../../volume.md) $V=\pi R^2h$ then fixes the radius. The [self-similar spreading of a viscous oil slick](../../../../../../self-similar-spreading-of-a-viscous-oil-slick.md) is

$$
\boxed{h(r,t)=\frac{6\mu}{\Delta\rho\,g\,t},\quad
u(r,t)=\frac r{2t},\quad
R(t)=\left(\frac{\Delta\rho\,g\,Vt}{6\pi\mu}\right)^{1/2},\qquad 0\leq r<R(t).}
$$

The point-release idealization is singular at $t=0$; a finite initial uniform slick gives the same solution with a time shift.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
