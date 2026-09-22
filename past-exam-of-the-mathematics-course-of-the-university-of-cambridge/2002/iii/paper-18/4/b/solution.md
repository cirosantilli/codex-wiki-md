<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a real [inner product space](../../../../../../inner-product-space.md) $V=\mathbb R^5$, define

$$
\Phi(u\wedge v)(w)=\langle v,w\rangle u-\langle u,w\rangle v.
$$

This map takes values in the [Special orthogonal Lie algebra](../../../../../../special-orthogonal-lie-algebra.md): its matrices are skew-symmetric. It sends $e_i\wedge e_j$ to $E_{ij}-E_{ji}$, so it is an isomorphism between the two ten-dimensional spaces. For $g\in SO(5)$, invariance of the inner product gives

$$
\Phi(gu\wedge gv)=g\Phi(u\wedge v)g^{-1}.
$$

This proves the [exterior square realization of the orthogonal adjoint representation](../../../../../../exterior-square-realization-of-the-orthogonal-adjoint-representation.md), including equivariance, rather than merely matching dimensions.

After complexification, part (a) is therefore the [weight decomposition](../../../../../../weight-decomposition.md) of the [Adjoint representation](../../../../../../adjoint-representation-of-a-lie-algebra.md). Its zero [weight space](../../../../../../weight-space.md) is the complex centralizer of $\mathfrak t$. The two zero-weight wedges are nonzero multiples of $e_1\wedge e_2$ and $e_3\wedge e_4$, which map under $\Phi$ to the two infinitesimal rotation generators of $T$. Hence

$$
Z_{\mathfrak{so}(5)}(\mathfrak t)=\mathfrak t.
$$

If a larger torus contained $T$, its Lie algebra would commute with $\mathfrak t$ and therefore lie in $\mathfrak t$. Equality of Lie algebras and connectedness of both tori force equality of the groups. Thus **$T$ is a maximal torus**.

Let $\varepsilon_j$ denote the real coordinate functional $x_j$. In the real weight convention, with the common factor $i$ removed from the differentiated torus weights, the [root system](../../../../../../root-system.md) is

$$
\boxed{\Phi=\{\pm\varepsilon_1,\pm\varepsilon_2,
\pm(\varepsilon_1+\varepsilon_2),\pm(\varepsilon_1-\varepsilon_2)\}.}
$$

These are the [roots of a root system](../../../../../../root-of-a-root-system.md) of type [B2 root system](../../../../../../b2-root-system.md). In the imaginary-valued compact Lie-algebra convention each displayed functional is multiplied by $i$. Every root space is one-dimensional, as part (a) explicitly shows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
