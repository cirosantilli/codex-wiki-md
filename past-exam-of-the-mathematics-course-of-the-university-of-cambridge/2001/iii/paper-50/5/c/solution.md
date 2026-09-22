<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On a region with smooth positive area, set $q=G(Z)Q(\theta,\zeta)$, $\zeta=h(Z)$. Substitution into the [simple wave](../../../../../../simple-wave.md) equation gives

$$
Gh'Q_\zeta-G^2QQ_\theta+\left(G'+\frac G2\frac{A'}A\right)Q=0.
$$

Remove the last term by $G'/G=-A'/(2A)$, and choose $h'=G$. Starting at a regular section $Z_0$, one convenient normalized [area transformation of a nonlinear acoustic simple wave](../../../../../../area-transformation-of-a-nonlinear-acoustic-simple-wave.md) is

$$
\boxed{G(Z)=\sqrt{\frac{A(Z_0)}{A(Z)}},\qquad \zeta=\int_{Z_0}^Z\sqrt{\frac{A(Z_0)}{A(s)}}\,ds.}
$$

In the notation $g(\zeta)$, set $g(\zeta)=G(h^{-1}(\zeta))$. The remaining equation is $Q_\zeta-QQ_\theta=0$. With initial value $f$ at $Z_0$, the [method of characteristics](../../../../../../method-of-characteristics.md) gives

$$
Q=f(\xi),\qquad \theta=\xi-f(\xi)\zeta,\qquad q=G(Z)f(\xi).
$$

The map from the initial label loses invertibility when $1-f'(\xi)\zeta=0$. For smooth data with bounded derivative and $M=\sup f'>0$, the first forward [characteristic crossing](../../../../../../characteristic-crossing.md) is at $\zeta_s=1/M$; if $M\leq0$, no forward shock occurs.

For spherical spreading, write physical radius as $R>0$ and specify data at an emitting radius $R_0>0$. Since $A(R)=R^2$,

$$
G=\frac{R_0}R,\qquad \zeta=R_0\log(R/R_0).
$$

The [shock distance for a spherical simple wave launched at finite radius](../../../../../../shock-distance-for-a-spherical-simple-wave-launched-at-finite-radius.md) is

$$
\boxed{R_s=R_0\exp\left(\frac1{R_0M}\right),\qquad M=\sup_\xi f'(\xi)>0.}
$$

If the axial distance is measured from the emitting surface, $Z=R-R_0$, then $A(Z)=(R_0+Z)^2$ and

$$
\boxed{Z_s=R_0\left[\exp\left(\frac1{R_0M}\right)-1\right].}
$$

No finite shock distance exists in this model when $M\leq0$.

The printed combination $A=Z^2$ with general bounded data at $Z=0$ is singular and does not define the intended outgoing spherical initial-value problem. Along a spherical characteristic, $d\theta/dR=-q$ and $dq/dR=-q/R$, so $Rq$ is constant. A bounded trace at $R=0$ forces that constant to be zero for every [characteristic curve](../../../../../../characteristic-curve.md) emanating from the origin; arbitrary nonzero bounded $f$ cannot be launched there. For example, the ostensibly admissible data $f\equiv1$ would demand both $Rq=0$ and a nonzero trace, a contradiction. The logarithmic transformed distance is also divergent at the origin. Thus an unqualified numerical shock formula from those literal data would be unjustified. The finite-radius formulas above give the physical interpretation once the launching radius, or the shifted area law, is supplied.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
