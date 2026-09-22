<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\delta=4-D$ and $F(g)=g-Cg^2/\delta+O(g^3)$. Since changing the arbitrary [renormalization scale](../../../../renormalization-scale.md) must leave the bare theory fixed,

$$
0=\mu\frac{d}{d\mu}\big[\mu^\delta F(g)\big]
=\mu^\delta\big[\delta F(g)+\beta(g)F'(g)\big].
$$

Write $\beta(g)=-\delta g+bg^2+O(g^3)$. Substitution gives, through order $g^2$,

$$
0=\delta g-Cg^2+(-\delta g+bg^2)
\left(1-\frac{2Cg}{\delta}\right)
=(b+C)g^2+O(g^3).
$$

Therefore $b=-C$, and the specified residue gives the [renormalization-group beta function](../../../../beta-function-physics.md)

$$
\boxed{\beta(g)=-(4-D)g+\frac3{16\pi^2}g^2+O(g^3).}
$$

The derivative is at fixed bare parameters. It does not say the physical theory changes when $\mu$ changes; the [running coupling](../../../../running-coupling.md) compensates the scale used to describe it. The coefficient also depends on defining the derivative with respect to $\log\mu$, rather than $\log\mu^2$; using the latter would divide both terms by two.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
