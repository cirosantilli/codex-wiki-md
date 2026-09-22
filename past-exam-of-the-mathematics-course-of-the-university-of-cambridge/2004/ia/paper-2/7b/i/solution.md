<h1 id="7b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here the [autonomous planar system](../../../../../../autonomous-planar-system.md) is $\dot x=v$, $\dot v=-\cos x$. Its [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are

$$
\boxed{(x_*,v_*)=(\pi/2+n\pi,0),\qquad n\in\mathbb Z.}
$$

The [Jacobian matrix](../../../../../../jacobian-matrix.md) is

$$
J_*=\begin{pmatrix}0&1\\ \sin x_*&0\end{pmatrix},
\qquad \mu^2=\sin x_*=(-1)^n.
$$

For even $n$, the [eigenvalues](../../../../../../eigenvalue.md) are $1,-1$, so these points are unstable [saddle equilibria](../../../../../../saddle-equilibrium.md). Writing $\xi=x-x_*$, their local unstable and stable directions are $v=\xi$ and $v=-\xi$ respectively. For odd $n$, the [eigenvalues](../../../../../../eigenvalue.md) are $i,-i$.

To classify the latter points nonlinearly, differentiate the [first integral](../../../../../../first-integral.md)

$$
H(x,v)=\frac{v^2}{2}+\sin x:
\qquad \dot H=v(-\cos x)+\cos x\,v=0.
$$

At $x_*=3\pi/2+2m\pi$ this [energy](../../../../../../energy.md) has a strict local minimum. Its nearby [level sets](../../../../../../level-set.md) are closed curves, proving that the odd-$n$ points are stable [center equilibria](../../../../../../center-equilibrium.md), with no attraction to the center. The [phase portrait](../../../../../../phase-portrait.md) consists of closed oscillatory orbits for $-1<H<1$, [heteroclinic orbits](../../../../../../heteroclinic-orbit.md) at $H=1$ joining consecutive [saddle equilibria](../../../../../../saddle-equilibrium.md), and open rotating orbits for $H>1$. The separating curves have

$$
v=\pm\sqrt{2(1-\sin x)}.
$$

Above the horizontal axis $\dot x=v>0$, so flow is rightward; below it flow is leftward. The closed orbits are clockwise, and these same signs orient every separating and rotating orbit.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [7B](../../7b.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2004](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
