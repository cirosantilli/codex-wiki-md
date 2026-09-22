<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Lie group](../../../../../lie-group.md) is a [group](../../../../../group-split.md) and [smooth manifold](../../../../../smooth-manifold.md) whose multiplication and inversion are smooth. A [Lie algebra](../../../../../lie-algebra-split.md) is a [vector space](../../../../../vector-space-split.md) with a bilinear alternating bracket satisfying the [Jacobi identity](../../../../../jacobi-identity.md). For a [Matrix Lie group](../../../../../matrix-lie-group.md) $G\subset GL(m,\mathbb C)$, a [logarithmic chart of a matrix Lie group](../../../../../logarithmic-chart-of-a-matrix-lie-group.md) near $g$ sends $h$ to $\log(g^{-1}h)\in\mathfrak g=T_I G$; the [matrix exponential](../../../../../matrix-exponential.md) is its local inverse, and the [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md) makes the local group operations smooth.

For $B_1,B_2\in\mathfrak g$, consider the group commutator

$$
C(s,t)=e^{sB_1}e^{tB_2}e^{-sB_1}e^{-tB_2}\in G.
$$

Its logarithm takes values in the vector space $\mathfrak g$, and expansion at $(0,0)$ gives

$$
\frac{\partial^2}{\partial s\,\partial t}\bigg|_{(0,0)}\log C(s,t)
=B_1B_2-B_2B_1.
$$

Thus $\mathfrak g$ is closed under the [commutator](../../../../../commutator.md). Bilinearity, alternation, and the Jacobi identity follow from matrix multiplication, so this proves that the [Lie algebra of a matrix Lie group](../../../../../lie-algebra-of-a-matrix-lie-group.md) has

$$
\boxed{[B_1,B_2]=B_1B_2-B_2B_1.}
$$

A [principal bundle](../../../../../principal-bundle.md) $\pi:P\to M$ with structure group $G$ is a smooth [fiber bundle](../../../../../fiber-bundle-split.md) with a free right $G$-action, each fiber a single orbit, and equivariant local trivializations $\pi^{-1}(U)\cong U\times G$.

For the right action of the [unitary group](../../../../../unitary-group.md) on $GL(n,\mathbb C)$, define

$$
q(g)=\frac12\log(gg^*)\in H(n).
$$

The matrix $gg^*$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md) and a [Hermitian matrix](../../../../../hermitian-operator.md), and $q(gu)=q(g)$ for $u\in U(n)$. The [polar decomposition of an invertible complex matrix](../../../../../polar-decomposition-of-an-invertible-complex-matrix.md) gives the unique factorization

$$
g=e^{q(g)}u(g),
\qquad u(g)=e^{-q(g)}g\in U(n).
$$

Consequently

$$
\Phi:H(n)\times U(n)\longrightarrow GL(n,\mathbb C),
\qquad(B,u)\longmapsto e^Bu
$$

is a diffeomorphism. If $W\subset H(n)$ is a neighborhood of zero and $N=q^{-1}(W)$, then $N$ is an open neighborhood of $I$, it is a union of complete orbits, and

$$
V=\bigcup_{h\in N}R(h)=N\cong W\times U(n).
$$

Moreover, two matrices have the same value of $q$ exactly when they differ by right multiplication by a unitary matrix. Thus $q$ induces the smooth identification

$$
\boxed{M=GL(n,\mathbb C)/U(n)\cong H(n),}
$$

under which $\pi$ is projection $H(n)\times U(n)\to H(n)$. This is the [general linear group modulo the unitary group](../../../../../general-linear-group-modulo-the-unitary-group.md), and $\pi$ is in fact a globally trivial principal $U(n)$-bundle.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
