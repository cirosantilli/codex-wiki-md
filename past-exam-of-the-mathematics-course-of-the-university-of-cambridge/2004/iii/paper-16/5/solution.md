<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Over the [Grassmannian](../../../../../grassmannian.md) $\operatorname{Gr}_k(\mathbb C^N)$, the [complex tautological bundle on a Grassmannian](../../../../../complex-tautological-bundle-on-a-grassmannian.md) is

$$
\gamma_k^N=\{(W,v):W\in\operatorname{Gr}_k(\mathbb C^N),\ v\in W\},\qquad (W,v)\longmapsto W.
$$

Its fibre at $W$ is the k-plane $W$ itself. A neighbourhood of a fixed plane consists of graphs of linear maps $A:W\to W^\perp$; $(A,w)\mapsto(\operatorname{graph}A,w+Aw)$ gives a [local trivialization](../../../../../local-trivialization.md). The inclusions of coordinate spaces give the infinite [Grassmannian](../../../../../grassmannian.md) and its tautological rank-k bundle $\gamma_k^\infty$.

Use the customary compact Hausdorff base convention for the [classification of complex vector bundles by a Grassmannian](../../../../../classification-of-complex-vector-bundles-by-a-grassmannian.md); equivalently the argument uses finite subordinate partitions of unity. Give a rank-k [complex vector bundle](../../../../../complex-vector-bundle.md) $E\to X$ a continuous [fiber metric](../../../../../fiber-metric.md) given by Hermitian [inner products](../../../../../inner-product.md). Choose a finite trivializing cover with local orthonormal coordinates $t_i:E|_{U_i}\to U_i\times\mathbb C^k$, and a subordinate [partition of unity](../../../../../partition-of-unity.md) $\rho_i$ with support contained in $U_i$. Define

$$
J_x(v)=\bigl(\sqrt{\rho_i(x)}\,t_{i,x}(v)\bigr)_i\in\mathbb C^{kr},
$$

extending each component by zero off its support. This is continuous and satisfies $\|J_x(v)\|^2=\sum_i\rho_i(x)\|v\|^2=\|v\|^2$, so it is a fibrewise embedding. The image planes vary continuously: in local frames, their [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) is $J(J^*J)^{-1}J^*$. Thus they define a map $c_E:X\to\operatorname{Gr}_k(\mathbb C^{kr})$, and $v\mapsto(x,J_xv)$ identifies $E$ with $c_E^*\gamma_k^\infty$. This proves that every bundle is a tautological [pullback vector bundle](../../../../../pullback-vector-bundle.md), by the [finite-dimensional embedding of a complex vector bundle](../../../../../finite-dimensional-embedding-of-a-complex-vector-bundle.md).

We next prove the two independence assertions that turn this construction into a bijection. First, homotopic maps have isomorphic [pullback vector bundles](../../../../../pullback-vector-bundle.md). Pulling back along a [homotopy](../../../../../homotopy.md) gives a bundle over compact Hausdorff $X\times I$; embed that bundle in a finite [trivial vector bundle](../../../../../trivial-vector-bundle.md) by the construction just given. Its image has a continuous family of rank-k [orthogonal projection matrices](../../../../../orthogonal-projection-matrix.md) $P(x,t)$. [Compactness](../../../../../compact-space.md) gives a subdivision $0=t_0<\cdots<t_s=1$ with

$$
\|P(x,t_{j+1})-P(x,t_j)\|<1\qquad\text{for every }x.
$$

Restriction of $P(x,t_{j+1})$ to the image at $t_j$ is injective: if it killed $v$, then $v=(P(x,t_j)-P(x,t_{j+1}))v$, impossible by the strict norm bound unless $v=0$. Equal ranks make it an isomorphism, with continuous local inverses. Composing these bundle maps identifies the endpoint [vector bundles](../../../../../vector-bundle.md). The fact that [close orthogonal projections identify their image bundles](../../../../../close-orthogonal-projections-identify-their-image-bundles.md) therefore makes the pullback assignment well-defined on [homotopy](../../../../../homotopy.md) classes.

Conversely, suppose two classifying maps give isomorphic [vector bundles](../../../../../vector-bundle.md). The infinite [Grassmannian](../../../../../grassmannian.md) has its standard weak CW topology; the compact-subset property of [CW complexes](../../../../../cw-complex.md) puts the compact images of the two maps in finite stages. Their tautological [pullback vector bundles](../../../../../pullback-vector-bundle.md) therefore give two finite-dimensional embeddings $J_0:E\to\mathbb C^{N_0}$ and $J_1:E\to\mathbb C^{N_1}$ of the same bundle, after using the [vector bundle isomorphism](../../../../../vector-bundle-isomorphism.md). In orthogonal coordinate blocks interpolate by

$$
J_t(v)=\left(\cos\frac{\pi t}{2}\,J_0(v),\ \sin\frac{\pi t}{2}\,J_1(v)\right).
$$

At least one coefficient is nonzero, so every $J_t$ is injective and its image planes give a continuous [Grassmannian](../../../../../grassmannian.md) [homotopy](../../../../../homotopy.md). One endpoint uses the first block and the other the second block. Moving the latter coordinate copy to the standard one is a fixed unitary change of coordinates, connected to the identity by a path in the [unitary group](../../../../../unitary-group.md). Such a path exists by diagonalizing the [unitary matrix](../../../../../unitary-matrix.md) and continuously varying its [eigenvalue](../../../../../eigenvalue.md) phases. Hence the original two maps are homotopic in the infinite [Grassmannian](../../../../../grassmannian.md). This also proves independence of all embedding and metric choices. Together the two directions establish

$$
\boxed{\operatorname{Vect}_{\mathbb C}^k(X)\longleftrightarrow[X,\operatorname{Gr}_k(\mathbb C^\infty)],\qquad[f]\longmapsto[f^*\gamma_k^\infty].}
$$

For arbitrary non-Hausdorff compact spaces without the required numerability, that usual bundle-classification statement needs additional hypotheses; the construction above specifies precisely the conventional setting being used.

Write $B=\operatorname{Gr}_k(\mathbb C^\infty)$. For the assumed [fiber bundle](../../../../../fiber-bundle-split.md) $U_k\to\nu\to B$ with [contractible](../../../../../contractible-space.md) total space, the [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md) has segment

$$
0=\pi_q(\nu)\longrightarrow\pi_q(B)\xrightarrow{\partial}\pi_{q-1}(U_k)\longrightarrow\pi_{q-1}(\nu)=0.
$$

For $q\ge2$ this gives group isomorphisms. For $q=1$, the relevant pointed-set part and connectedness of $U_k$ give $\pi_1(B)=0$, corresponding to the single component $\pi_0(U_k)$. Thus the claimed formula includes its endpoint:

$$
\boxed{\pi_q(B)\cong\pi_{q-1}(U_k)\quad(q\ge1),\qquad\pi_1(B)=0.}
$$

Finally the determinant gives a [fiber bundle](../../../../../fiber-bundle-split.md) $SU_2\to U_2\to S^1$. Since $\pi_3(S^1)=\pi_4(S^1)=0$, its exact sequence yields $\pi_3(U_2)\cong\pi_3(SU_2)$. The given identification $SU_2\cong S^3$ and the degree calculation $\pi_3(S^3)=\mathbb Z$ therefore give

$$
[S^4,B U_2]=\pi_4(B U_2)\cong\pi_3(U_2)\cong\mathbb Z.
$$

The equality of free and based [homotopy](../../../../../homotopy.md) classes uses the simple connectedness just proved. Hence

$$
\boxed{\operatorname{Vect}_{\mathbb C}^2(S^4)\cong\mathbb Z.}
$$

The classification of [rank-two complex vector bundles over the four-sphere](../../../../../rank-two-complex-vector-bundles-over-the-four-sphere.md) is a bijection of isomorphism classes, labelled by the integer [clutching function](../../../../../clutching-function.md) [homotopy](../../../../../homotopy.md) class after choosing a generator. It is not an assertion that [Whitney sum](../../../../../whitney-sum-of-vector-bundles.md) gives a group operation on bundles of fixed rank two.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
