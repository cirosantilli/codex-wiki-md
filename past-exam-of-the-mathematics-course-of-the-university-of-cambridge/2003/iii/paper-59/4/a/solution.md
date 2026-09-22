<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $r>0$, polar coordinates give $\dot r=r(\mu_1-2x)$ and $\dot\theta=1$; the remaining amplitude equation is $\dot x=\mu_2+x^2+r^2$. Interpret $r=0$ in the original complex coordinate, where the phase is undefined.

If $\mu_2<0$, put $a=\sqrt{-\mu_2}$. The full [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are $E_\pm:(z,x)=(0,\pm a)$. Their [eigenvalues](../../../../../../eigenvalue.md) are

$$
E_+:\quad 2a,\ \mu_1-2a\pm i,\qquad
E_-:\quad -2a,\ \mu_1+2a\pm i.
$$

Thus $E_-$ is stable for $\mu_1<-2a$ and has a two-dimensional [unstable manifold](../../../../../../unstable-manifold.md) for $\mu_1>-2a$. The point $E_+$ has a one-dimensional [unstable manifold](../../../../../../unstable-manifold.md) for $\mu_1<2a$ and is repelling for $\mu_1>2a$. On $\mu_2=0$ they merge in a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md); the simultaneous zero and imaginary [eigenvalues](../../../../../../eigenvalue.md) at $(\mu_1,\mu_2)=(0,0)$ give a [fold-Hopf bifurcation](../../../../../../fold-hopf-bifurcation.md).

A steady positive amplitude represents a full [periodic orbit](../../../../../../periodic-orbit.md), not a full equilibrium. Solving the amplitude equations gives

$$
\boxed{x_*=\mu_1/2,\qquad r_*^2=-\mu_2-\mu_1^2/4,\qquad \text{period}=2\pi.}
$$

It exists in the wedge $\mu_2<-\mu_1^2/4$. The transverse amplitude [Jacobian matrix](../../../../../../jacobian-matrix.md) has characteristic polynomial $s^2-\mu_1s+4r_*^2$. Its two transverse [Floquet exponents](../../../../../../floquet-exponent.md) have negative real part for $\mu_1<0$ and positive real part for $\mu_1>0$; the phase direction supplies the neutral [Floquet multiplier](../../../../../../floquet-multiplier.md) one.

The wedge boundaries are [Hopf bifurcations](../../../../../../hopf-bifurcation.md) at $\mu_1=-2a$ from $E_-$ and $\mu_1=2a$ from $E_+$. The left branch is supercritical, producing a stable [periodic orbit](../../../../../../periodic-orbit.md) as $E_-$ loses stability; the right branch is subcritical in the oscillatory subspace, with an unstable [periodic orbit](../../../../../../periodic-orbit.md) on the side where the transverse complex pair of $E_+$ is stable. The real unstable direction of $E_+$ persists throughout. There are no full [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) when $\mu_2>0$, and $\dot x>0$ then excludes a local [periodic orbit](../../../../../../periodic-orbit.md). The right panel of the [bifurcation diagram](../../../../../../bifurcation-diagram.md) in part 1(b) shows the primary curves and the perturbed global curve calculated below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
