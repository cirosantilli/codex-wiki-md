<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [differential form](../../../../../differential-form-split.md) of degree $k$ is integrated over an oriented $k$-dimensional [smooth manifold](../../../../../smooth-manifold.md) by integrating its coefficient in orientation-preserving coordinates. For an oriented parametrization $F:U\to M$, this means integrating the [pullback](../../../../../pullback-category-theory.md) $F^*\alpha$ over $U$; a [partition of unity](../../../../../partition-of-unity.md) combines charts. The [change of variables formula](../../../../../change-of-variables-formula.md) makes the result independent of the charts. Reversing the [orientation of a smooth manifold](../../../../../orientation-of-a-smooth-manifold.md) reverses the integral. The [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) says, for a compact oriented $k$-dimensional [smooth manifold](../../../../../smooth-manifold.md) with boundary and a smooth $(k-1)$-form $\beta$,

$$
\int_M d\beta=\int_{\partial M}\beta,
$$

where the right-hand side includes the boundary [pullback](../../../../../pullback-category-theory.md), and the boundary has the [outward-normal-first boundary orientation](../../../../../outward-normal-first-boundary-orientation.md). Compact support suffices on a noncompact manifold. This unifies the fundamental theorem of calculus, circulation and flux identities.

For example, take the unit disk $D$ oriented by $dx\wedge dy$ and the [differential one-form](../../../../../one-form.md) $\beta=\tfrac12(x\,dy-y\,dx)$. Its [exterior derivative](../../../../../exterior-derivative.md) is $d\beta=dx\wedge dy$, so the area integral is $\pi$. Parametrizing the positively oriented circle by $(x,y)=(\cos t,\sin t)$ gives the [pullback](../../../../../pullback-category-theory.md) $\beta=\tfrac12dt$ and the boundary integral $\int_0^{2\pi}\tfrac12dt=\pi$, directly illustrating [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md).

For the distance calculation, write $u=|\mathbf r_1|$, $v=|\mathbf r_2|$, $x=u+v$ and $y=u-v$; these are scalar radii, not position vectors. The [triangle inequality](../../../../../triangle-inequality.md) and its reverse give $r\leq u+v=x$ and $|y|=|u-v|\leq r$. Also,

$$
x+|y|=2\max(u,v)\leq2R.
$$

Thus **$r\leq x\leq2R-|y|$ and $|y|\leq r$**. These conditions, with $u,v\geq0$, are also sufficient for a triangle with side lengths $u,v,r$. Endpoints correspond to collinear configurations.

Assume the two positions are [independent random variables](../../../../../independent-random-variables.md), each having constant volume [probability density](../../../../../probability-density.md) inside the radius-$R$ [ball](../../../../../ball-mathematics.md). Independence is needed: uniform marginal distributions alone do not determine the distance distribution. Put $C=3/(4\pi R^3)$ and $\mathbf s=\mathbf r_2-\mathbf r_1$. The [change of variables](../../../../../change-of-variables-formula.md) $(\mathbf r_1,\mathbf r_2)\mapsto(\mathbf r_1,\mathbf s)$ has unit [Jacobian determinant](../../../../../jacobian-determinant.md), so the joint probability volume [differential form](../../../../../differential-form-split.md) is the product of the two normalized volume forms. In spherical coordinates for $\mathbf r_1$ and for $\mathbf s$ relative to its axis, it is

$$
C^2u^2\sin\theta_1\,du\wedge d\theta_1\wedge d\phi_1\wedge r^2\sin\theta\,dr\wedge d\theta\wedge d\chi.
$$

The polar coordinates fail on axes and at zero radii, which are sets of zero volume and do not affect the [probability](../../../../../probability.md). Here $\theta$ is the angle from $\mathbf r_1$ to $\mathbf s$. The [law of cosines](../../../../../law-of-cosines.md) becomes

$$
v^2=u^2+r^2+2ur\cos\theta.
$$

Differentiating and taking the [wedge product](../../../../../exterior-product.md) with $du\wedge dr$ eliminates the terms involving $du$ and $dr$:

$$
du\wedge dr\wedge(v\,dv)=-ur\sin\theta\,du\wedge dr\wedge d\theta.
$$

Consequently the positive integration density transforms by $|\sin\theta\,d\theta|=v\,dv/(ur)$ at fixed $u,r$. The minus sign is accounted for by reversal of limits: $v$ decreases as $\theta$ increases. The radial variable retained is $r$, while the polar angle is replaced by $v$; equivalently one can start with the angle between the two position vectors and replace that angle by $r$. The wording of the printed hint conflates these two coordinate choices, but its volume form gives the stated transformation directly.

Integrating $\sin\theta_1\,d\theta_1\,d\phi_1$ over the first orientation gives $4\pi$, and integrating $d\chi$ gives $2\pi$. The [probability density function](../../../../../probability-density-function.md) of $r$ is therefore

$$
f_R(r)=8\pi^2C^2r\iint_{D_r}uv\,du\,dv=\frac{9r}{2R^6}\iint_{D_r}uv\,du\,dv,
$$

where $D_r$ has $0\leq u,v\leq R$ and $|u-v|\leq r\leq u+v$. There are no such configurations for $r>2R$.

To evaluate this integral explicitly, the [Jacobian determinant](../../../../../jacobian-determinant.md) of $(u,v)=((x+y)/2,(x-y)/2)$ has absolute value $1/2$. Hence $uv\,du\,dv=(x^2-y^2)\,dx\,dy/8$ as a positive density. For $0\leq r\leq2R$, set $a=\min(r,2R-r)$. The domain is $-a\leq y\leq a$, $r\leq x\leq2R-|y|$, and evenness in $y$ gives

$$
I(r)=\iint_{D_r}uv\,du\,dv=\frac14\int_0^a\left[\frac{(2R-y)^3-r^3}{3}-y^2(2R-y-r)\right]dy.
$$

An antiderivative, zero at $y=0$, yields

$$
I(r)=\frac1{12}\left[(8R^3-r^3)a-6R^2a^2+ra^3+\frac{a^4}{2}\right].
$$

Substituting $a=r$ for $r\leq R$ and $a=2R-r$ for $r\geq R$ gives the same polynomial in both intervals:

$$
I(r)=\frac{2R^3r}{3}-\frac{R^2r^2}{2}+\frac{r^4}{24}.
$$

Thus the [distance between two uniform points in a three-dimensional ball](../../../../../distance-between-two-uniform-points-in-a-three-dimensional-ball.md) has the final density

$$
\boxed{dP=\left(\frac{3r^2}{R^3}-\frac{9r^3}{4R^4}+\frac{3r^5}{16R^6}\right)dr,\qquad 0\leq r\leq2R.}
$$

It is zero outside this interval. Its nonnegativity also follows from $f_R(r)=3r^2(4R+r)(2R-r)^2/(16R^6)$, and direct integration gives $\int_0^{2R}f_R(r)dr=1$. The derivation uses the full six-dimensional probability volume [differential form](../../../../../differential-form-split.md), rather than treating the three scalar distances as independent.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
