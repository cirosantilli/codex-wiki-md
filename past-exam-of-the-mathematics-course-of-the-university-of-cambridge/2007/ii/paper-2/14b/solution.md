<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

For the Laplace-type contour ansatz, differentiating under the integral and putting $P(t)=t^2-t-2$ gives the differential-equation residual

$$
\int_\gamma e^{zt}\{zP(t)f(t)+(2-t)f(t)\}\,dt.
$$

[Integration by parts](../../../../../integration-by-parts.md) turns this into $[e^{zt}Pf]_{\partial\gamma}+\int_\gamma e^{zt}[(2-t)f-(Pf)']dt$. Thus it vanishes whenever the endpoint contribution vanishes and $(Pf)'=(2-t)f$. The latter condition is $Pf'=3(1-t)f$, solved by

$$
f(t)=\frac1{(t-2)(t+1)^2}
$$

up to a constant multiplier. Closed contours avoiding the poles make the endpoint contribution zero.

Choose separate positively oriented small circles around 2 and $-1$. The [residue theorem](../../../../../residue-theorem.md) gives, after division by $2\pi i$,

$$
\operatorname{Res}_{t=2}(e^{zt}f)=\frac{e^{2z}}9,\qquad
\operatorname{Res}_{t=-1}(e^{zt}f)=-\frac{(3z+1)e^{-z}}9.
$$

Therefore

$$
\boxed{w(z)=Ae^{2z}+B(3z+1)e^{-z}.}
$$

The [Wronskian](../../../../../wronskian.md) of the two basis functions is $-9ze^z$, nonzero for $z\ne0$. They span the two-dimensional solution space on every regular domain, and both extend entire across the apparent singular point at zero. Their initial values satisfy $w(0)=A+B$ and $w'(0)=2(A+B)$. Thus **every solution has $w'(0)=2w(0)$**, and the requested combination $w(0)=0$, $w'(0)\ne0$ is impossible. No additional logarithmic solution is lost: the two independent functions already span the solution space away from zero.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
