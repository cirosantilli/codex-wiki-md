<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For fixed source $(\xi,\eta)\in D$, define the [Dirichlet Green function](../../../../dirichlet-green-function.md) by $-\Delta_{x,y}G=\delta_{(\xi,\eta)}$ in $D$, $G=0$ on $\partial D$. It is [harmonic](../../../../harmonic-function.md) away from the source and has [singularity](../../../../complex-singularity.md) $-(2\pi)^{-1}\log\sqrt{(x-\xi)^2+(y-\eta)^2}$. The outward [normal vector](../../../../normal-vector.md) [derivative](../../../../derivative.md) is $\partial_nG=\mathbf n\cdot\nabla_{x,y}G$ at a boundary point of arc-length parameter $s$.

[Green's second identity](../../../../green-second-identity.md) gives $\int_D(u\Delta G-G\Delta u)=\int_{\partial D}(u\partial_nG-G\partial_nu)\,ds$. Substituting the two PDEs and the boundary data yields

$$
-u(\xi,\eta)+\int_DfG=\int_{\partial D}g\partial_nG,\qquad
\boxed{u(\xi,\eta)=-\int_{\partial D}g\partial_nG\,ds+\int_DfG\,dx\,dy.}
$$

The singular version follows by excising a small source disk and taking its radius to zero, or directly by the distributional identity.

For the upper half-plane use the opposite-sign image source at $(\xi,-\eta)$:

$$
\boxed{G=\frac1{4\pi}\log\frac{(x-\xi)^2+(y+\eta)^2}{(x-\xi)^2+(y-\eta)^2}.}
$$

The image lies outside the domain, so it is [harmonic](../../../../harmonic-function.md) inside; the true source has the required unit [singularity](../../../../complex-singularity.md), and the two distances agree at $y=0$, giving zero boundary value. On that boundary $\mathbf n=-\mathbf e_y$, so

$$
\partial_nG=-\frac\eta{\pi[(s-\xi)^2+\eta^2]}.
$$

The assumed far-field decay makes the large semicircle contribution vanish. With $f=0$, the representation becomes

$$
\boxed{u(\xi,\eta)=\frac\eta\pi\int_{-\infty}^\infty\frac{g(s)}{(\xi-s)^2+\eta^2}\,ds.}
$$

Finally set $s=\xi+\eta\tan\theta$, $ds=\eta\sec^2\theta\,d\theta$. The [Jacobian matrix](../../../../jacobian-matrix.md) cancels the denominator, giving

$$
\boxed{u(\xi,\eta)=\frac1\pi\int_{-\pi/2}^{\pi/2}g(\xi+\eta\tan\theta)\,d\theta.}
$$

If $g$ is even, the substitution $s\mapsto-s$ in the [Poisson integral](../../../../poisson-integral.md) gives $u(-\xi,\eta)=u(\xi,\eta)$. At $\eta=0$ this agrees with the continuous even boundary trace.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
