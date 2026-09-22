<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the unhalved geodesic [Lagrangian](../../../../lagrangian.md)

$$
\mathcal L=-c^2\alpha\dot t^2+\alpha^{-1}\dot r^2+r^2\dot\theta^2+r^2\sin^2\theta\dot\phi^2.
$$

The cyclic coordinates $t,\phi$ give $d(2c^2\alpha\dot t)/d\lambda=0$ and $d(2r^2\sin^2\theta\dot\phi)/d\lambda=0$. The other two [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
\frac d{d\lambda}(2r^2\dot\theta)-2r^2\sin\theta\cos\theta\dot\phi^2=0,
$$



$$
\frac d{d\lambda}\left(\frac{2\dot r}{\alpha}\right)+c^2\alpha'\dot t^2+\frac{\alpha'}{\alpha^2}\dot r^2-2r\dot\theta^2-2r\sin^2\theta\dot\phi^2=0.
$$

These reproduce the supplied geodesic equations. Expanding the derivatives and comparing with $\ddot x^\mu+\Gamma^\mu{}_{\nu\rho}\dot x^\nu\dot x^\rho=0$, in coordinates $(t,r,\theta,\phi)$, gives all nonzero [Christoffel symbols](../../../../christoffel-symbol.md):

$$
\boxed{\begin{aligned}
\Gamma^t{}_{tr}=\Gamma^t{}_{rt}&=\frac{\alpha'}{2\alpha},&
\Gamma^r{}_{tt}&=\frac{c^2\alpha\alpha'}2,&
\Gamma^r{}_{rr}&=-\frac{\alpha'}{2\alpha},\\
\Gamma^r{}_{\theta\theta}&=-r\alpha,&
\Gamma^r{}_{\phi\phi}&=-r\alpha\sin^2\theta,&
\Gamma^\theta{}_{r\theta}=\Gamma^\theta{}_{\theta r}&=\frac1r,\\
\Gamma^\phi{}_{r\phi}=\Gamma^\phi{}_{\phi r}&=\frac1r,&
\Gamma^\theta{}_{\phi\phi}&=-\sin\theta\cos\theta,&
\Gamma^\phi{}_{\theta\phi}=\Gamma^\phi{}_{\phi\theta}&=\cot\theta.
\end{aligned}}
$$

Here $\alpha'=-2r/r_S^2$. This is the [static patch of de Sitter spacetime](../../../../static-patch-of-de-sitter-spacetime.md), with $0\leq r<r_S$ for the stationary observers used below. Apparent divergences at the polar axis, origin or horizon belong to the chosen coordinate chart; they are not themselves evidence of a curvature singularity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
