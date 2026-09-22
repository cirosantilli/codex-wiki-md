<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [integer](../../../../../integer.md) coefficients. The [mapping-torus homology from Mayer–Vietoris](../../../../../mapping-torus-homology-from-mayer-vietoris.md) works for every [continuous map](../../../../../continuous-map.md) $f:X\to X$, without assuming that the [mapping torus](../../../../../mapping-torus.md) is a [fiber bundle](../../../../../fiber-bundle-split.md). Project to the time [circle](../../../../../circle.md) and choose two open arcs, one containing the seam and one away from it. The inverse image $U$ of the seam arc is a [mapping cylinder](../../../../../mapping-cylinder.md) neighborhood with a [deformation retraction](../../../../../deformation-retraction.md) to its target copy of $X$; the inverse image $V$ of the other arc is a product with a [deformation retraction](../../../../../deformation-retraction.md) to $X$. Their intersection has two components, each with a [deformation retraction](../../../../../deformation-retraction.md) to $X$. Label the upper component first. With the convention that the second inclusion in the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) has a minus sign, its [homology](../../../../../homology-split.md) map is

$$
H_q(X)\oplus H_q(X)\longrightarrow H_q(X)\oplus H_q(X),\qquad (a,b)\longmapsto(a+f_*b,-a-b).
$$

Indeed, the upper component includes into the seam neighborhood by the identity, while retracting the lower component across the seam applies $f$. Put $u=a+b$ and $v=b$, and replace target coordinates $(p,q)$ by $(p+q,-q)$. The map becomes $((f_*-\operatorname{id})v,u)$. Negating $v$ gives a [direct sum](../../../../../direct-sum.md) of $\operatorname{id}-f_*$ and an [isomorphism](../../../../../isomorphism.md). Canceling the latter summands in the long [exact sequence](../../../../../exact-sequence.md) yields

$$
\boxed{\cdots\longrightarrow H_q(X)\xrightarrow{\operatorname{id}-f_*}H_q(X)\longrightarrow H_q(T_f)\longrightarrow H_{q-1}(X)\xrightarrow{\operatorname{id}-f_*}H_{q-1}(X)\longrightarrow\cdots.}
$$

In particular, there is a [short exact sequence](../../../../../short-exact-sequence.md)

$$
0\longrightarrow\operatorname{coker}(\operatorname{id}-f_*|_{H_q})\longrightarrow H_q(T_f)\longrightarrow\ker(\operatorname{id}-f_*|_{H_{q-1}})\longrightarrow0.
$$

No splitting of this [short exact sequence](../../../../../short-exact-sequence.md) is assumed at this stage.

For the [torus](../../../../../torus.md), take the coordinate loops $c_1(t)=[(t,0)]$ and $c_2(t)=[(0,t)]$ as the [basis](../../../../../basis.md) of $H_1$. Their lifts to $\mathbb R^2$ have endpoint displacements $e_1,e_2$. Applying $A$ changes those displacements to its columns, so

$$
(f_A)_*[c_j]=\sum_i A_{ij}[c_i].
$$

This also follows from the identification of the [first homology group](../../../../../first-homology.md) with the [abelianization](../../../../../abelianization.md) of the [fundamental group](../../../../../fundamental-group.md). The [Künneth theorem](../../../../../kunneth-theorem.md) gives $H_2(X)=\mathbb Z$, with generator the product [orientation class](../../../../../fundamental-class.md). If $\alpha,\beta$ are the dual degree-one [cohomology](../../../../../cohomology-split.md) classes, then $\alpha\smile\beta$ evaluates to one on this generator, and

$$
f_A^*(\alpha\smile\beta)=(A_{11}\alpha+A_{12}\beta)\smile(A_{21}\alpha+A_{22}\beta)=\det(A)\,\alpha\smile\beta.
$$

Thus the degree-two [homology](../../../../../homology-split.md) map is multiplication by $\det A$, as in [homology of an integer torus endomorphism](../../../../../homology-of-an-integer-torus-endomorphism.md). The claim that the [torus](../../../../../torus.md) map is a [homeomorphism](../../../../../homeomorphism.md) requires $A$ to be a [unimodular matrix](../../../../../unimodular-matrix.md), equivalently an [integer](../../../../../integer.md) inverse or $\det A=\pm1$; nonsingularity over $\mathbb R$ alone would only give a [covering map](../../../../../covering-space.md) of finite degree. The particular [matrix](../../../../../matrix.md) here is unimodular.

For this [matrix](../../../../../matrix.md), $\det A=1$ and

$$
I-A=\begin{pmatrix}1&-1\\1&1\end{pmatrix}.
$$

Its [kernel](../../../../../kernel-of-a-linear-map.md) is zero and its [Smith normal form](../../../../../smith-normal-form.md) is $\operatorname{diag}(1,2)$, so its [cokernel](../../../../../cokernel.md) is $\mathbb Z/2$. The maps $\operatorname{id}-f_*$ on $H_0$ and $H_2$ are zero. Substituting into the [short exact sequences](../../../../../short-exact-sequence.md), and splitting the degree-one extension because its quotient $\mathbb Z$ is free, gives

$$
\boxed{H_q(T_{f_A};\mathbb Z)\cong\begin{cases}\mathbb Z,&q=0,2,3,\\\mathbb Z\oplus\mathbb Z/2,&q=1,\\0,&\text{otherwise}.\end{cases}}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
