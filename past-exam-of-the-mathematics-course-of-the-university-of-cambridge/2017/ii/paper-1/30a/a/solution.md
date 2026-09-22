<h1 id="30a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The equilibrium equations are $x(-1+x^2+\beta y^2)=y(-1+\beta x^2+y^2)=0$. For $\beta\ne1$ the [fixed points](../../../../../../fixed-point.md) are the origin, four axis points $(\pm1,0),(0,\pm1)$, and four diagonal points $(\pm s,\pm s)$ with independent signs and $s=(1+\beta)^{-1/2}$. The hypothesis $\beta>-1$ ensures that $s$ is real. The [Jacobian matrix](../../../../../../jacobian-matrix.md) has diagonal entries $-1+3x^2+\beta y^2$, $-1+\beta x^2+3y^2$ and off-diagonal entries $2\beta xy$.

At the origin both [eigenvalues](../../../../../../eigenvalue.md) are $-1$, so it is a [stable node](../../../../../../stable-node.md). At each axis point the [eigenvalues](../../../../../../eigenvalue.md) are $2,\beta-1$. At each diagonal point they are $2,2(1-\beta)/(1+\beta)$, along the radial and transverse diagonal directions respectively. Thus

$$
\boxed{\begin{array}{c|cc}
&-1<\beta<1&\beta>1\\\hline
\text{origin}&\text{sink}&\text{sink}\\
\text{axis points}&\text{saddles}&\text{sources}\\
\text{diagonal points}&\text{sources}&\text{saddles}
\end{array}}.
$$

The axes and diagonals are invariant lines. For $\beta=1/2$ the axis [saddle points](../../../../../../saddle-point.md) have stable directions transverse to their axes and unstable directions along them; the diagonal points are [unstable nodes](../../../../../../unstable-node.md). For $\beta=2$ these roles switch: the diagonal [saddle points](../../../../../../saddle-point.md) have stable transverse directions and unstable radial directions, and the axis points are [unstable nodes](../../../../../../unstable-node.md). Their [stable manifolds](../../../../../../stable-manifold.md) separate trajectories attracted to the origin from outward-escaping trajectories. Symmetry gives the other quadrants.

For $\beta=1$, the entire unit circle consists of equilibria. In [polar coordinates](../../../../../../polar-coordinates.md) $\dot r=r(r^2-1)$ and $\dot\theta=0$: every ray inside the circle moves toward the origin, and every ray outside moves outward. The circle has neutral tangential and unstable radial directions; its points are not isolated [saddle points](../../../../../../saddle-point.md) or [unstable nodes](../../../../../../unstable-node.md).

All three [phase portraits](../../../../../../phase-portrait.md) are shown below. The potential $\Phi=-(x^2+y^2)/2+(x^4+y^4)/4+\beta x^2y^2/2$ satisfies $(\dot x,\dot y)=\nabla\Phi$ and $\dot\Phi=|\nabla\Phi|^2$, ruling out nonconstant periodic orbits. Blue curves show the saddle stable [separatrices](../../../../../../separatrix.md), integrated backwards from their local stable directions. The flow arrows and invariant lines, together with the equilibrium classification, specify the topology of the sketches.

<a id="30a/a/image-phase-portraits-and-equilibrium-branches"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1-phase-portraits.png)

**[Figure 1](#30a/a/image-phase-portraits-and-equilibrium-branches). Phase portraits and equilibrium branches**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30A](../../30a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
