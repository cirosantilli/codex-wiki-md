<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

Assume the integrand is sufficiently [smooth](../../../../../smooth-function.md) near the positive admissible profiles. Define the [second variation](../../../../../second-variation.md) as $\delta^2F[y,\xi]=\left.d^2F[y+\varepsilon\xi]/d\varepsilon^2\right|_{\varepsilon=0}$, so it is twice the quadratic Taylor coefficient. Differentiation under the integral gives

$$
\delta^2F=\int_\alpha^\beta\left(f_{yy}\xi^2+2f_{yp}\xi\xi'+f_{pp}\xi'^2\right)dx,\qquad p=y'.
$$

Integrating the middle term by parts, with $\xi(\alpha)=\xi(\beta)=0$, yields

$$
\boxed{\delta^2F=\int_\alpha^\beta\left[\left(f_{yy}-\frac d{dx}f_{yp}\right)\xi^2+f_{pp}\xi'^2\right]dx}.
$$

All coefficients are evaluated along $y$.

For the surface-area integrand $f=2\pi y\sqrt{1+p^2}$, the [Beltrami identity](../../../../../beltrami-identity.md) for a stationary profile reads

$$
f-pf_p=\frac{2\pi y}{\sqrt{1+y'^2}}=2\pi E.
$$

Equivalently, its [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $yy''=1+y'^2$, solved by the positive [catenoid](../../../../../catenoid.md) profile $y=E\cosh((x-x_0)/E)$ with $E>0$. Equal boundary radii at $x=\pm L$, for $L>0$, require $x_0=0$, so

$$
\boxed{y(x)=E\cosh(x/E),\qquad a=E\cosh(L/E)}.
$$

Direct substitution also verifies the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). This is a stationary profile whenever a positive $E$ satisfying the boundary relation exists; such an $E$ does not exist for arbitrary ring separations and radii.

On this profile, with $z=x/E$, the coefficients are $f_{yy}=0$, $f_{pp}=2\pi E\operatorname{sech}^2z$ and $d f_{yp}/dx=(2\pi/E)\operatorname{sech}^2z$. Changing variables therefore gives

$$
\boxed{\delta^2F=2\pi\int_{-L/E}^{L/E}(\xi_z^2-\xi^2)\operatorname{sech}^2z\,dz}.
$$

The printed strict inequality must mean **every nonzero admissible variation**: the zero function makes the integral zero, so the literal quantifier including it is false.

For completeness, the strict positivity here is sufficient for a strict local minimum in the fixed-endpoint $C^1$ topology, among positive axisymmetric graph profiles. On this finite interval the weight $p(z)=\operatorname{sech}^2z$ has a positive minimum. The regular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) associated with $Q[\xi]=\int p(\xi_z^2-\xi^2)$ has an attained lowest [Dirichlet eigenvalue](../../../../../dirichlet-eigenvalue.md) $\lambda_1$ in the [Rayleigh quotient](../../../../../rayleigh-quotient.md). Its first [eigenfunction](../../../../../eigenfunction.md) is a nonzero [smooth](../../../../../smooth-function.md) admissible variation; the assumed strict positivity gives $\lambda_1>0$. Hence $Q\geq\lambda_1\|\xi\|_{L^2}^2$. Combining this with $Q\geq p_{\min}\|\xi_z\|_{L^2}^2-p_{\max}\|\xi\|_{L^2}^2$ proves [coercivity](../../../../../coercive-function.md) in the [Sobolev space](../../../../../sobolev-space-split.md) $H_0^1$.

The coefficients of the [second variation](../../../../../second-variation.md) depend continuously on $(y,y')$ while $y>0$. For a sufficiently small $C^1$ perturbation, the quadratic forms along the segment from the stationary profile to the perturbed one retain a uniform positive [coercivity](../../../../../coercive-function.md) bound. Taylor's formula with integral remainder, and the vanishing [first variation](../../../../../first-variation.md), then gives $F[y+v]-F[y]\geq c\|v\|_{H^1}^2>0$ for nonzero sufficiently small admissible $v$. **The stationary area is therefore a strict local minimum under the stated nonzero-variation condition**. This supplies the uniform bound needed in an infinite-dimensional problem, rather than relying on pointwise positivity alone in an arbitrary function space.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
