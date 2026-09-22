<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

The [diffusive flux](../../../../../diffusive-flux.md) is $\mathbf J=-D\nabla C$ by [Fick's first law](../../../../../fick-s-first-law.md). Conservation in any fixed control volume $V$ gives $\frac d{dt}\int_V C=-\int_{\partial V}\mathbf J\cdot\mathbf n+\int_V F$. The [divergence theorem](../../../../../divergence-theorem.md) and arbitrariness of $V$ yield

$$
\boxed{C_t=\nabla\cdot(D\nabla C)+F.}
$$

After the initial point injection, $F=0$ and $D=kC$ with $k>0$, so radial symmetry gives $C_t=k r^{-2}(r^2CC_r)_r$. Total mass is $4\pi\int_0^\infty r^2C\,dr=4\pi M$.

A spreading radius $R$ and typical concentration obey $CR^3\sim M$ and $R^2\sim kCt$. Thus $R^5\sim Mkt$. In the proposed ansatz this gives

$$
\boxed{\alpha=\frac25,\quad\beta=\frac35,\quad\gamma=\frac15,\qquad
C=M^{2/5}(kt)^{-3/5}f(\xi),\quad\xi=\frac r{(Mkt)^{1/5}}.}
$$

Direct substitution, including the time derivative of $\xi$, gives

$$
-\frac35f-\frac15\xi f'=\frac1{\xi^2}(\xi^2ff')'.
$$

Multiplying by $\xi^2$ makes the left side $-(\xi^3f)'/5$. Regularity and zero radial flux at the origin set the integration constant to zero, so $ff'=-\xi f/5$. On the positive region $f'= -\xi/5$. Nonnegativity, compact support and continuity at its edge give

$$
f(\xi)=\frac{(\xi_0^2-\xi^2)_+}{10}.
$$

Its normalization is $1=\int_0^{\xi_0}\xi^2f\,d\xi=\xi_0^5/75$. Therefore the [spherical nonlinear-diffusion source profile](../../../../../spherical-nonlinear-diffusion-source-profile.md) is

$$
\boxed{f(\xi)=\frac{(75^{2/5}-\xi^2)_+}{10},\qquad
r_0(t)=(75Mkt)^{1/5}.}
$$

The concentration and flux vanish at the free boundary, so there is no distributional flux jump despite the derivative kink. The solution satisfies the diffusion equation weakly across that boundary and classically inside its positive region. Its support shrinks to the origin as $t\downarrow0$, and testing against a continuous compactly supported function gives the limit $4\pi M$ times its value at zero. This verifies the prescribed point injection as well as the mass normalization.

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
