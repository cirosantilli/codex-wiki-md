<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Take $\lambda=e^{\pi i/3}$ and the chosen $s=e^{\pi i/6}$. Then $\lambda s=i$, so $i/(\lambda s)=1$, and $-1/\lambda=\lambda^2$. In affine coordinates the chosen lift becomes

$$
\upsilon(x,y)=(1+\lambda^2x,y).
$$

Since $\lambda^2$ is a primitive cube root of unity, $1+\lambda^2+\lambda^4=0$. Three iterations fix $x$ and $y$, whereas one does not. Thus

$$
\boxed{\operatorname{ord}(\upsilon)=3\quad\text{for the lift chosen above}.}
$$

The other square-root choice replaces this map by $(x,y)\mapsto(1+\lambda^2x,-y)$. Its cube is $(x,y)\mapsto(x,-y)$, so that lift has order six. This sign dependence is why a lift was specified explicitly.

Both fix the point at infinity. In the [complex torus](../../../../complex-torus.md) model their linear multipliers have order three or six, so the [lattice](../../../../lattice.md) is stable under a primitive cube root $\zeta=e^{2\pi i/3}$ and hence under $e^{\pi i/3}=1+\zeta$. Choose a shortest nonzero period $\omega$. The triangular [lattice](../../../../lattice.md) $\mathbb Z+\zeta\mathbb Z$ has covering radius $1/\sqrt3<1$: its equilateral triangles of side one each have circumradius $1/\sqrt3$. Approximating any period divided by $\omega$ by this [lattice](../../../../lattice.md) leaves a strictly shorter period, which must be zero. Therefore

$$
\boxed{\Lambda=\omega(\mathbb Z+e^{\pi i/3}\mathbb Z).}
$$

Thus the cubic has the hexagonal [lattice](../../../../lattice.md) shape, independently of which of the two lifts is chosen.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
