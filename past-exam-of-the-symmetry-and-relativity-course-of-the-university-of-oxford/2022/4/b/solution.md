<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With constant [rest mass](../../../../invariant-mass.md), $\mathbf p=m\gamma\mathbf v$ and the [chain rule](../../../../chain-rule.md) gives $\dot\gamma=\gamma^3(\mathbf v\cdot\mathbf a)/c^2$. Hence the laboratory [relativistic force](../../../../relativistic-force.md) is

$$
\mathbf F=m\gamma\mathbf a+\frac{m\gamma^3}{c^2}(\mathbf v\cdot\mathbf a)\mathbf v.
$$

Use the [vector triple product identity](../../../../vector-triple-product.md) $\mathbf v\times(\mathbf v\times\mathbf a)=\mathbf v(\mathbf v\cdot\mathbf a)-v^2\mathbf a$, and $\gamma^3(1-v^2/c^2)=\gamma$, to obtain

$$
\boxed{\mathbf F=m\gamma^3\left(\mathbf a+\frac{\mathbf v\times(\mathbf v\times\mathbf a)}{c^2}\right).}
$$

The [relativistic energy](../../../../relativistic-energy.md) is $E=m\gamma c^2$, whose [time derivative](../../../../time-derivative.md) is $m\gamma^3\mathbf v\cdot\mathbf a$. Taking the [dot product](../../../../dot-product.md) of the first expression for $\mathbf F$ with $\mathbf v$ gives the same quantity, because $\gamma+\gamma^3v^2/c^2=\gamma^3$. Thus $dE/dt=\mathbf F\cdot\mathbf v$. Since $d/d\tau=\gamma\,d/dt$, the [four-force](../../../../four-force.md) is

$$
\boxed{F^\alpha=\frac{dp^\alpha}{d\tau}=\left(\frac{\gamma\mathbf F\cdot\mathbf v}{c},\gamma\mathbf F\right).}
$$

Its [tensor contraction](../../../../tensor-contraction.md) with the [four-velocity](../../../../four-velocity.md) vanishes: $F^\alpha U_\alpha=-\gamma^2\mathbf F\cdot\mathbf v+\gamma^2\mathbf F\cdot\mathbf v=0$. This [orthogonality](../../../../orthogonal-vectors.md) also follows by differentiating $p^\alpha p_\alpha=-m^2c^2$. Resolving the laboratory [acceleration](../../../../acceleration.md) relative to $\mathbf v$ gives $\mathbf F_\parallel=m\gamma^3\mathbf a_\parallel$ and $\mathbf F_\perp=m\gamma\mathbf a_\perp$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
