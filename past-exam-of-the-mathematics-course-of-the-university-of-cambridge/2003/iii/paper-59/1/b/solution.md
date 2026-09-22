<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use local coordinates $q=\theta-\pi/2$, $p=\phi$ at $P_1$. The [Jacobian matrix](../../../../../../jacobian-matrix.md), its [trace](../../../../../../matrix-trace.md) and its [determinant](../../../../../../determinant.md) are

$$
J=\begin{pmatrix}\lambda-1&-2\\1-\kappa&-2\end{pmatrix},\qquad T=\lambda-3,\qquad D=2(2-\lambda-\kappa).
$$

Consequently $P_1$ is attracting when $T<0,D>0$, repelling when $T>0,D>0$, and a [saddle equilibrium](../../../../../../saddle-equilibrium.md) when $D<0$. A transition between a [node](../../../../../../node-dynamical-systems.md) and a [focus](../../../../../../focus-dynamical-systems.md) at $T^2=4D$ changes the linear geometry but is not a [bifurcation](../../../../../../bifurcation.md) of the local topological [phase portrait](../../../../../../phase-portrait.md).

The [stationary bifurcation](../../../../../../stationary-bifurcation.md) curve is $\lambda+\kappa=2$. To identify it, write $C=\cos2\phi$, $S=\sin2\phi$. At a non-equatorial [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md), eliminating $S$ gives

$$
C=\frac{\lambda+\kappa}{2},\qquad \cos\theta=\frac{2S}{\kappa-\lambda}.
$$

Near $(3,-1)$, if $d=2-\lambda-\kappa>0$, these yield $p=\pm\sqrt d/2+O(d^{3/2})$ and $q=p+o(\sqrt d)$. The two branches are related by the local reflection $(q,p)\mapsto(-q,-p)$. Their [determinants](../../../../../../determinant.md) are $-4d+o(d)$, so they are [saddle equilibria](../../../../../../saddle-equilibrium.md). This is a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md); on the portion with $T<0$ the saddle branches lie on the side where $P_1$ is stable, giving a [subcritical pitchfork bifurcation](../../../../../../subcritical-pitchfork-bifurcation.md).

A [Hopf bifurcation](../../../../../../hopf-bifurcation.md) requires $T=0,D>0$, hence

$$
\boxed{\lambda=3,\quad\kappa<-1.}
$$

The oscillation frequency is $\omega=\sqrt{-2(1+\kappa)}$. At the intersection $\boxed{(\lambda,\kappa)=(3,-1)}$, $J\ne0$ but $J^2=0$: there is a double zero [eigenvalue](../../../../../../eigenvalue.md) with one [eigenvector](../../../../../../eigenvector.md). The map from $(\lambda,\kappa)$ to $(T,D)$ has nonzero [Jacobian determinant](../../../../../../jacobian-determinant.md), so two independent parameter conditions produce this [codimension-two bifurcation](../../../../../../codimension-two-bifurcation.md). Reflection removes quadratic terms; the appropriate initial comparison is with a [reflection-symmetric cubic double-zero normal form](../../../../../../reflection-symmetric-cubic-double-zero-normal-form.md), subject to the cubic degeneracy checked below.

For completeness, the printed [vector field](../../../../../../vector-field.md) has a subcritical, rather than supercritical, [Hopf bifurcation](../../../../../../hopf-bifurcation.md). In the mechanical coordinates $x=p$, $y=\dot p$, at $\lambda=3$ its cubic acceleration has $x^2y$ coefficient $b=6(\kappa-3)(\kappa+1)/(\kappa-1)^2$ and $y^3$ coefficient $d_3=-2/(\kappa-1)^2$. For a small harmonic oscillation, the averaged cubic change of $H=(y^2+\omega^2x^2)/2$ is $\omega^2A^4(b+3d_3\omega^2)/8$, where

$$
b+3d_3\omega^2=\frac{6(\kappa+1)}{\kappa-1}>0.
$$

Thus a small unstable [periodic orbit](../../../../../../periodic-orbit.md) lies on the attracting side of the [Hopf bifurcation](../../../../../../hopf-bifurcation.md). This calculation matters when comparing the original equations with the later assumed [normal form](../../../../../../normal-form-dynamical-systems.md).

<a id="1/b/image-local-bifurcation-curves-for-the-spherical-system-rotating-convection-and-the-fold-hopf-system"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-59-bifurcation-diagrams.png)

**[Figure 1](#1/b/image-local-bifurcation-curves-for-the-spherical-system-rotating-convection-and-the-fold-hopf-system). Local bifurcation curves for the spherical system, rotating convection, and the fold–Hopf system**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
