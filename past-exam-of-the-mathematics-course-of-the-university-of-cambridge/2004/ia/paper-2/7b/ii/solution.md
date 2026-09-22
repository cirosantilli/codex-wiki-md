<h1 id="7b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For both parameters the [autonomous planar system](../../../../../../autonomous-planar-system.md) is $\dot x=v$, $\dot v=-x(x^2+\lambda x+1)$. It has the conserved [energy](../../../../../../energy.md)

$$
H=\frac{v^2}{2}+V_\lambda(x),\qquad
V_\lambda(x)=\frac{x^4}{4}+\frac{\lambda x^3}{3}+\frac{x^2}{2}.
$$

Indeed $\dot H=v\dot v+V_\lambda'(x)\dot x=0$. At any [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) $(x_*,0)$ the [eigenvalues](../../../../../../eigenvalue.md) satisfy

$$
\mu^2=-V_\lambda''(x_*)=-(3x_*^2+2\lambda x_*+1).
$$

For $\lambda=1$, the quadratic $x^2+x+1$ is strictly positive, so the only [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) is $(0,0)$, with [eigenvalues](../../../../../../eigenvalue.md) $\pm i$. Since $V_1'(x)$ has the sign of $x$, $V_1$ has a unique strict minimum at zero and tends to infinity in both directions. All positive [energy](../../../../../../energy.md) levels are closed curves surrounding this stable [center equilibrium](../../../../../../center-equilibrium.md). They are clockwise: rightward when $v>0$ and leftward when $v<0$.

For $\lambda=5/2$, factor $x^2+(5/2)x+1=(x+2)(x+1/2)$. The three [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) and their classifications are

$$
\boxed{\begin{array}{c|c|c}
(x_*,0)&\text{eigenvalues}&\text{type}\\\hline
(-2,0)&\pm i\sqrt3&\text{center}\\
(-1/2,0)&\pm\sqrt3/2&\text{saddle}\\
(0,0)&\pm i&\text{center}
\end{array}}
$$

The two [center equilibria](../../../../../../center-equilibrium.md) are stable but not asymptotically stable; the [saddle equilibrium](../../../../../../saddle-equilibrium.md) is unstable. At the [saddle equilibrium](../../../../../../saddle-equilibrium.md) the local unstable and stable directions are $v=(\sqrt3/2)(x+1/2)$ and $v=-(\sqrt3/2)(x+1/2)$.

The potential values are $V(-2)=-2/3$, $V(0)=0$, and $V(-1/2)=7/192$. Consequently there are closed loops around the left center for $-2/3<H<0$, closed loops in both wells for $0<H<7/192$, and a figure-eight pair of [homoclinic orbits](../../../../../../homoclinic-orbit.md) at $H=7/192$. At $H=0$ the right center is a stationary point while the left well still has a closed orbit. For $H>7/192$, each closed curve encircles both centers and the saddle.

The two [homoclinic orbits](../../../../../../homoclinic-orbit.md) satisfy $v=\pm\sqrt{2(7/192-V(x))}$. Their outer turning points can be located exactly from

$$
V(x)-\frac7{192}=\frac{(2x+1)^2(12x^2+28x-7)}{192},
\qquad
x_{\rm L,R}=\frac{-7\mp\sqrt{70}}6.
$$

Every nonstationary [energy](../../../../../../energy.md) curve is oriented to the right in the upper half-plane and to the left in the lower half-plane. The sketches show the closed curves, the separating orbits, the stable and unstable saddle directions and the direction of flow.

<a id="7b/ii/image-clockwise-phase-flows-alternating-pendulum-saddles-and-centers-and-the-one-well-and-two-well-quartic-potentials"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2-phase-portraits.png)

**[Figure 2](#7b/ii/image-clockwise-phase-flows-alternating-pendulum-saddles-and-centers-and-the-one-well-and-two-well-quartic-potentials). Clockwise phase flows, alternating pendulum saddles and centers, and the one-well and two-well quartic potentials**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
