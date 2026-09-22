<h1 id="12a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $r_0$ is an interior point and choose $\varepsilon$ small enough that its closed ball lies inside $V$. Apply [Green's second identity](../../../../../../green-second-identity.md) to the punctured region $V_\varepsilon=V\setminus\overline{B_\varepsilon(r_0)}$, where the potential $\psi=1/|r-r_0|$ is smooth and satisfies [Laplace equation](../../../../../../laplace-equation.md). Since $\nabla^2\phi=-\rho$, this gives

$$
\int_{V_\varepsilon}\frac{\rho(r)}{|r-r_0|}\,dV
=\int_S(\phi\partial_n\psi-\psi\partial_n\phi)\,dS
+\int_{S_\varepsilon}(\phi\partial_{n_\varepsilon}\psi-\psi\partial_{n_\varepsilon}\phi)\,dS.
$$

The crucial orientation is the outward unit [normal vector](../../../../../../normal-vector.md) of the punctured region: on the inner [sphere](../../../../../../sphere.md), it is $n_\varepsilon=-e_r$, pointing toward $r_0$. Consequently $\psi=1/\varepsilon$ and $\partial_{n_\varepsilon}\psi=1/\varepsilon^2$. The inner boundary term becomes

$$
\int_{S_\varepsilon}\left(\frac{\phi}{\varepsilon^2}+\frac1\varepsilon\partial_r\phi\right)dS.
$$

Writing $r=r_0+\varepsilon\omega$ and $dS=\varepsilon^2d\Omega$, its first part tends to $\int_{|\omega|=1}\phi(r_0)\,d\Omega=4\pi\phi(r_0)$ by continuity. The second part is $O(\varepsilon)$ because the [gradient](../../../../../../gradient.md) of $\phi$ is bounded near $r_0$, and hence tends to zero.

The omitted volume term also tends to zero: for bounded $\rho$ near $r_0$, its absolute value is bounded by a constant times $4\pi\int_0^\varepsilon r\,dr=O(\varepsilon^2)$. Thus the limiting [integral](../../../../../../integral.md) exists, and rearranging the outer boundary terms gives

$$
\boxed{4\pi\phi(r_0)
=\int_V\frac{\rho(r)}{|r-r_0|}\,dV
+\int_S\left[\frac1{|r-r_0|}\partial_n\phi
-\phi\partial_n\frac1{|r-r_0|}\right]dS.}
$$

This is [Green's third identity](../../../../../../green-s-third-identity.md) for the [Poisson equation](../../../../../../poisson-equation.md) with the stated sign convention. It retains both boundary terms; no homogeneous boundary condition has been assumed. The punctured-domain calculation accounts for the singular source without incorrectly applying the regular [divergence theorem](../../../../../../divergence-theorem.md) through $r_0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12A](../../12a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
