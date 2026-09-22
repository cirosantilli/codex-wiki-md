<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use symmetric positive conductivity, for example $\alpha I\preceq a(x)\preceq MI$ with $\alpha>0$. Let $v$ have the same [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) as $u$, and write $v=u+\phi$ with $\phi\in H_0^1(\Omega)$. [Symmetry](../../../../../../symmetry-physics.md) gives

$$
J(v)=J(u)+2\int_\Omega\nabla\phi\cdot a\nabla u\,dx
+\int_\Omega\nabla\phi\cdot a\nabla\phi\,dx.
$$

The middle integral vanishes by the weak field equation; equivalently integrate by parts, use $\phi=0$ on the boundary and $\nabla\cdot(a\nabla u)=0$. Hence

$$
J(v)-J(u)=\int_\Omega\nabla\phi\cdot a\nabla\phi\,dx
\ge\alpha\int_\Omega|\nabla\phi|^2\,dx\ge0.
$$

Therefore

$$
\boxed{J(u)=\min_{\ v|_{\partial\Omega}=\lambda\cdot x}J(v).}
$$

Equality forces $\nabla\phi=0$, and its zero boundary trace gives $\phi=0$, proving uniqueness. This is the [Dirichlet principle](../../../../../../dirichlet-principle.md) for the conductivity equation.

The positivity is essential to the physical minimum-energy interpretation; [symmetry](../../../../../../symmetry-physics.md) by itself would give only stationarity. For example, take $a=-I$, $\lambda=0$ and $u=0$. The field equation holds, but every nonzero smooth compactly supported $v$ has $J(v)=-\int_\Omega|\nabla v|^2<0$, and scaling $v$ makes the energy unbounded below. Thus if the printed word “conductivity” were not understood to include positivity, the stated minimum claim would require that additional hypothesis.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
