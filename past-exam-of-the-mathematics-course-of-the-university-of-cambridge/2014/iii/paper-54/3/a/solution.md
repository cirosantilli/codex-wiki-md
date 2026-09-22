<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For steady spherical [polytropic flow](../../../../../../polytropic-flow.md), write $u=u_r$ and use the [polytropic equation of state](../../../../../../polytropic-equation-of-state.md) $p=K\rho^\gamma$, with $K>0$. Mass conservation and radial [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) are

$$
\frac{d}{dr}(r^2\rho u)=0,\qquad uu'=-\frac{p'}\rho-\frac{GM}{r^2},\qquad c_s^2=\frac{dp}{d\rho}=\gamma K\rho^{\gamma-1}.
$$

The mass equation gives $\rho'/\rho=-2/r-u'/u$. Substitute it into momentum balance to obtain

$$
\boxed{\frac{u^2-c_s^2}{u}u'=\frac{2c_s^2}{r}-\frac{GM}{r^2}.}
$$

At a [sonic point](../../../../../../sonic-point.md) the derivative coefficient vanishes. A smooth finite-slope solution must make the numerator vanish there too:

$$
\boxed{u_c^2=c_{s,c}^2,\qquad r_c=\frac{GM}{2c_{s,c}^2}.}
$$

Finally $dp/\rho=d[\gamma K\rho^{\gamma-1}/(\gamma-1)]$. Integrating momentum gives the [Bernoulli equation](../../../../../../bernoulli-equation.md)

$$
\boxed{\frac{u^2}{2}+\frac{\gamma p}{(\gamma-1)\rho}-\frac{GM}{r}=C.}
$$

This is [kinetic energy](../../../../../../kinetic-energy.md) plus [specific enthalpy](../../../../../../specific-enthalpy.md) plus gravitational potential per unit mass. The [polytropic stellar wind](../../../../../../polytropic-stellar-wind.md) selects a particular transonic branch of these equations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
