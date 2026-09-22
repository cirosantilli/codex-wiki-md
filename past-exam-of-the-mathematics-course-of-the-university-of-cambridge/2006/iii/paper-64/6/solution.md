<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Marsden-Weinstein theorem](../../../../../marsden-weinstein-theorem.md) needs a [Hamiltonian action](../../../../../hamiltonian-group-action.md), not merely an action by [symplectomorphisms](../../../../../symplectomorphism.md). Assume an equivariant [moment map](../../../../../moment-map.md) $\mu:P\to\mathfrak g^*$ exists, choose a coadjoint-fixed [regular value](../../../../../regular-value.md) $a$ (zero is the usual choice), and assume the action on $C=\mu^{-1}(a)$ is free and proper. Regularity makes $C$ a [submanifold](../../../../../submanifold.md) of codimension $g=\dim G$. Equivariance and invariance of $a$ make $C$ invariant under $G$, and freeness and properness give a smooth quotient $P'=C/G$. Thus

$$
\boxed{\dim P'=(2n-g)-g=2n-2g.}
$$

Let $\iota:C\hookrightarrow P$ and $\pi:C\to P'$. For $v\in T_pC$ and $\xi\in\mathfrak g$,

$$
\omega(\xi_P,v)=d\mu_\xi(v)=0.
$$

Moreover the conormal of $C$ is spanned by the independent $d\mu_\xi$, so nondegeneracy of $\omega$ gives $(T_pC)^\omega=\{\xi_P(p)\}$. The coadjoint-fixed value makes these orbit directions tangent to $C$. Hence the kernel of $\iota^*\omega$ is exactly the orbit tangent space. The restricted form is invariant and horizontal, so descends uniquely to a [two-form](../../../../../2-form.md) $\omega'$ with

$$
\boxed{\pi^*\omega'=\iota^*\omega.}
$$

It is closed because $\omega$ is closed. If a quotient tangent vector annihilates $\omega'$, any lift lies in the kernel just identified and is vertical; the quotient vector is therefore zero. This proves nondegeneracy and completes [symplectic reduction](../../../../../symplectic-reduction.md).

If the action is not free, singular strata or orbifold phenomena may occur. At a general noncentral [regular value](../../../../../regular-value.md) one quotients by its coadjoint stabilizer $G_a$, not by all of $G$; the regular dimension is $2n-g-\dim G_a$. These are genuine hypotheses behind the stated dimension formula.

Both proposed examples can be given explicitly. For [symplectic reduction of an isotropic oscillator](../../../../../symplectic-reduction-of-an-isotropic-oscillator.md), take two modes with

$$
\omega=\sum_{j=1}^2dq_j\wedge dp_j,\qquad
H=\frac12\sum_{j=1}^2(q_j^2+p_j^2),\qquad z_j=q_j+ip_j.
$$

Its [Hamiltonian flow](../../../../../hamiltonian-flow.md) is $z_j\mapsto e^{-it}z_j$, a circle action with [moment map](../../../../../moment-map.md) $H$. For $E>0$, $H^{-1}(E)$ is the sphere $S^3$ of radius $\sqrt{2E}$, and the action is free. The [Hopf fibration](../../../../../hopf-fibration.md) identifies its quotient with $\mathbb{CP}^1\cong S^2$. On the chart $z_1\ne0$, use $w=z_2/z_1$ and choose a section with $z_1=\sqrt{2E/(1+|w|^2)}$ real positive. Pulling back $\omega$ to this section gives

$$
\boxed{\omega'=\frac{iE\,dw\wedge d\bar w}{(1+|w|^2)^2}.}
$$

Writing $w=x+iy$ gives $2E\,dx\wedge dy/(1+x^2+y^2)^2$, whose integral is $2\pi E$. This is the [Fubini-Study form](../../../../../fubini-study-form.md) scaled by $E$ in the convention of area $2\pi$ at unit scale. The reduced dimension is $4-2=2$. At $E=0$, the circle fixes the origin and the smooth regular-level hypotheses fail.

For a unit-mass free particle in the plane, use the rotation circle action with angular-momentum [moment map](../../../../../moment-map.md) $\ell=xp_y-yp_x$. Choose $\ell_0\ne0$ so the entire level avoids $r=0$ and the action is free. Polar canonical coordinates have

$$
p_x\,dx+p_y\,dy=p_r\,dr+\ell\,d\theta,\qquad
\omega=dr\wedge dp_r+d\theta\wedge d\ell.
$$

Fixing $\ell=\ell_0$ and quotienting the rotation angle leaves

$$
\boxed{P'=T^*\mathbb R_{>0},\qquad\omega'=dr\wedge dp_r,\qquad
H'=\frac12p_r^2+\frac{\ell_0^2}{2r^2}.}
$$

This [planar rotational symplectic reduction](../../../../../planar-rotational-symplectic-reduction.md) replaces a planar free trajectory by radial motion with the centrifugal potential. A nonzero moment value is allowed because the circle is abelian and every value is coadjoint-fixed.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
