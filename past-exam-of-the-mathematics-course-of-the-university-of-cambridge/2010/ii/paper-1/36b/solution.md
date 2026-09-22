<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

For an affine parameter, the [geodesic equation](../../../../../geodesic-equation.md) is

$$
\boxed{\ddot x^a+\Gamma^a_{bc}\dot x^b\dot x^c=0.}
$$

Vary the energy action with endpoint-fixed variations. Its Euler-Lagrange equation is

$$
2g_{ab}\ddot x^b+2\partial_cg_{ab}\dot x^c\dot x^b
-\partial_ag_{bc}\dot x^b\dot x^c=0.
$$

Multiplying by $g^{da}/2$ and symmetrizing the velocity indices determines the [Levi-Civita connection](../../../../../levi-civita-connection.md):

$$
\boxed{\Gamma^d_{bc}=\frac12g^{da}
(\partial_bg_{ac}+\partial_cg_{ab}-\partial_ag_{bc}).}
$$

This determines the torsion-free metric connection; an antisymmetric-in-$b,c$ addition could not be detected by the geodesic energy variation alone.

For the displayed metric on $t>0$, the nonzero coefficients are $\Gamma^x_{xt}=\Gamma^x_{tx}=-1/t$ and $\Gamma^t_{xx}=\Gamma^t_{tt}=-1/t$. Consequently

$$
\ddot x-2\dot x\dot t/t=0,\qquad
\ddot t-(\dot x^2+\dot t^2)/t=0.
$$

For a timelike curve choose [proper time](../../../../../proper-time.md) so $(\dot x^2-\dot t^2)/t^2=-1$. The first equation integrates to $\dot x=pt^2$, and then $\dot t^2=t^2+p^2t^4$. If $p\ne0$, dividing and integrating gives

$$
x=x_c\pm\sqrt{t^2+p^{-2}},\qquad
\boxed{t^2=x^2+\alpha x+\beta,\quad
\alpha=-2x_c,\quad\beta=x_c^2-p^{-2}.}
$$

The timelike condition is $\alpha^2-4\beta=4p^{-2}>0$, with the appropriate branch in the coordinate patch. Conversely these curves with that condition obey the first integrals and admit a timelike affine parametrization.

There is an omitted family in the printed claim: if $p=0$, then **$x=x_c$ is a timelike vertical geodesic**, with $t=t_*e^{\pm\tau}$ in [proper time](../../../../../proper-time.md). No fixed finite $\alpha,\beta$ can represent all points of such a vertical curve by the displayed quadratic. The quadratic therefore describes the nonvertical [timelike geodesics](../../../../../timelike-geodesic.md); the vertical family must be included for completeness.

Together the two families describe the [timelike geodesics of an inverse-time conformal metric](../../../../../timelike-geodesics-of-an-inverse-time-conformal-metric.md).

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
