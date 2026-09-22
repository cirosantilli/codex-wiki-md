<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Order the [simple roots](../../../../simple-root.md) of the [G2 root system](../../../../g2-root-system.md) with $\alpha_1$ long and $\alpha_2$ short. This ordering is consistent with the supplied projection in [solution](../d/solution.md); reversing the nodes would interchange the two fundamental [Dynkin labels](../../../../dynkin-label.md). Choose $(\alpha_1,\alpha_1)=2$, $(\alpha_2,\alpha_2)=2/3$, and $(\alpha_1,\alpha_2)=-1$. With the same row convention for the [Cartan matrix](../../../../cartan-matrix.md) as in [solution](../a/solution.md),

$$
\boxed{A_{G_2}=\begin{pmatrix}2&-3\\-1&2\end{pmatrix},\qquad
\alpha_1=(2,-3),\quad\alpha_2=(-1,2).}
$$

The [positive roots](../../../../positive-root.md), with their [Dynkin labels](../../../../dynkin-label.md), are

$$
\begin{array}{c|c|c}
\text{root}&\text{Dynkin labels}&\text{length type}\\\hline
\alpha_2&(-1,2)&\text{short}\\
\alpha_1+\alpha_2&(1,-1)&\text{short}\\
\alpha_1+2\alpha_2&(0,1)&\text{short}\\
\alpha_1&(2,-3)&\text{long}\\
\alpha_1+3\alpha_2&(-1,3)&\text{long}\\
2\alpha_1+3\alpha_2&(1,0)&\text{long}
\end{array}
$$

For the [highest weight](../../../../highest-weight-of-a-representation.md) $(0,1)$, a lowering chain is

$$
(0,1)\xrightarrow{-\alpha_2}(1,-1)
\xrightarrow{-\alpha_1}(-1,2)
\xrightarrow{-\alpha_2}(0,0)
\xrightarrow{-\alpha_2}(1,-2)
\xrightarrow{-\alpha_1}(-1,1)
\xrightarrow{-\alpha_2}(0,-1).
$$

The middle three terms form the length-three [weight string](../../../../weight-string.md) for the short [simple root](../../../../simple-root.md). The [Weyl dimension formula](../../../../weyl-dimension-formula.md), with this long-first convention, is

$$
\dim V(a,b)=\frac{(a+1)(b+1)(a+b+2)(2a+b+3)(3a+b+4)(3a+2b+5)}{120}.
$$

It gives seven for $(0,1)$, so the chain exhausts the [weight system](../../../../weight-system.md), with every [weight multiplicity](../../../../weight-multiplicity.md) equal to one:

$$
\boxed{\mathbf7=(0,1):\quad(0,0),\quad
\pm(0,1),\quad\pm(1,-1),\quad\pm(-1,2).}
$$

For $(1,0)$, observe that $2\alpha_1+3\alpha_2=(1,0)$ is the [highest root](../../../../highest-root.md). Thus this is the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md); the twelve [root spaces](../../../../root-space.md) contribute the twelve nonzero [weights](../../../../weight-representation-theory.md) once, and the rank-two [Cartan subalgebra](../../../../cartan-subalgebra.md) contributes two zero [weights](../../../../weight-representation-theory.md). Therefore

$$
\boxed{\mathbf{14}=(1,0):\quad
\pm(2,-3),\ \pm(-1,3),\ \pm(1,0),\
\pm(-1,2),\ \pm(1,-1),\ \pm(0,1),\ (0,0)^{[2]}.}
$$

The same [Weyl dimension formula](../../../../weyl-dimension-formula.md) gives fourteen, confirming the count.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
