<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Rescale the ambient coordinates by $q_i=a_i r_i$. For each $i\in\{1,\ldots,n+1\}$ and $\varepsilon\in\{1,-1\}$, take the relatively open set $U_i^\varepsilon$ where $\varepsilon q_i>0$. Define a [manifold chart](../../../../../manifold-chart.md) by retaining all the $q_j$ except $q_i$:

$$
\phi_i^\varepsilon(r)=(q_1,\ldots,\widehat{q_i},\ldots,q_{n+1})\in B^n.
$$

Here $B^n$ is the open unit [open unit ball](../../../../../open-unit-ball.md). The inverse of this [manifold chart](../../../../../manifold-chart.md) is explicit:

$$
r_j=\frac{x_j}{a_j}\quad(j\ne i),\qquad r_i=\frac{\varepsilon}{a_i}\sqrt{1-\sum_{j\ne i}x_j^2}.
$$

The coordinate labels in $x$ retain their original indices. All the $a_i$ are nonzero, so this inverse exists; the strictly positive radicand makes it smooth on the whole open [open unit ball](../../../../../open-unit-ball.md). Projection and this inverse are continuous, so each [manifold chart](../../../../../manifold-chart.md) is a [homeomorphism](../../../../../homeomorphism.md) onto an open subset of $\mathbb R^n$.

These $2(n+1)$ [manifold charts](../../../../../manifold-chart.md) cover the [ellipsoid](../../../../../ellipsoid.md), because at every point at least one $q_i$ is nonzero. On an overlap with a different chart $U_j^\eta$, the coordinates of $\phi_j^\eta\circ(\phi_i^\varepsilon)^{-1}$ are the retained $x_k$ for $k\ne i,j$ together with

$$
q_i=\varepsilon\sqrt{1-\sum_{k\ne i}x_k^2}.
$$

Its domain is the open subset $\eta x_j>0$ of $B^n$. The displayed functions, and the reverse transition functions obtained by exchanging $i,j$, are smooth. Transitions between identical charts are the identity; opposite-sign charts with the same omitted coordinate do not overlap. The ambient subspace topology is [Hausdorff](../../../../../hausdorff-space.md) and [second countable](../../../../../second-countable-space.md), as it is inherited from Euclidean space. Thus this [coordinate-projection atlas of an ellipsoid](../../../../../coordinate-projection-atlas-of-an-ellipsoid.md) is a [smooth atlas](../../../../../smooth-atlas.md), proving **the ellipsoid is a smooth manifold of dimension $n$**. The rescaling $r\mapsto q$ also gives a [diffeomorphism](../../../../../diffeomorphism.md) with the unit [sphere](../../../../../sphere.md) $S^n$.

For the [three-sphere](../../../../../three-sphere.md), use its identification with [SU(2)](../../../../../su-2-group.md) rather than separate local constructions. With the [Pauli matrices](../../../../../pauli-matrices.md) $\tau_i$, put $T_i=-i\tau_i$. These form a real basis of the [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md) and satisfy

$$
T_iT_j=-\delta_{ij}I+\epsilon_{ijk}T_k.
$$

For $q_0^2+q_1^2+q_2^2+q_3^2=1$, the identification [SU(2) as the three-sphere](../../../../../su-2-as-the-three-sphere.md) is

$$
U(q)=q_0I+q_iT_i=\begin{pmatrix}q_0-iq_3&-q_2-iq_1\\q_2-iq_1&q_0+iq_3\end{pmatrix}.
$$

The matrix is unitary with determinant one. Conversely, every [SU(2) matrix](../../../../../su-2-matrix.md) has this form, and both the correspondence and its inverse are smooth.

The left translations $L_g(h)=gh$ are [diffeomorphisms](../../../../../diffeomorphism.md). Define three [left-invariant vector fields](../../../../../left-invariant-vector-field.md) by

$$
\boxed{X_i(g)=(dL_g)_eT_i=gT_i,\qquad i=1,2,3.}
$$

Matrix multiplication makes these [vector fields](../../../../../vector-field.md) smooth globally. Since $(dL_g)_e$ is an isomorphism from the [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md) to $T_g\mathrm{SU}(2)$, the three vectors are linearly independent at every point, and each is nowhere zero. This is the [parallelization of a Lie group by left translations](../../../../../parallelization-of-a-lie-group-by-left-translations.md).

Transporting the [left-invariant vector fields](../../../../../left-invariant-vector-field.md) to the [three-sphere](../../../../../three-sphere.md) gives the [quaternionic left-invariant frame on the three-sphere](../../../../../quaternionic-left-invariant-frame-on-the-three-sphere.md):

$$
\begin{aligned}
X_1(q)&=(-q_1,q_0,q_3,-q_2),\\
X_2(q)&=(-q_2,-q_3,q_0,q_1),\\
X_3(q)&=(-q_3,q_2,-q_1,q_0).
\end{aligned}
$$

Directly, $q\cdot X_i=0$ and $X_i\cdot X_j=\delta_{ij}$ on the unit [three-sphere](../../../../../three-sphere.md). Thus the vectors are tangent and form a global orthonormal [frame of a vector bundle](../../../../../frame-of-a-vector-bundle.md). **The three-sphere is a parallelizable manifold**, with [tangent bundle](../../../../../tangent-bundle.md) $TS^3\cong S^3\times\mathbb R^3$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
