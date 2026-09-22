<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Lie algebra representation](../../../../../lie-algebra-representation.md) $V$ is completely reducible when it is a [direct sum](../../../../../direct-sum.md) of irreducible [submodules](../../../../../submodule.md). In finite dimension this is equivalent to saying that every [submodule](../../../../../submodule.md) $W\subseteq V$ has an invariant complementary subspace. Indeed, one may split off a minimal nonzero [submodule](../../../../../submodule.md) and induct on dimension; conversely, if $V$ is a finite sum of simple [submodules](../../../../../submodule.md), choose a maximal sum $U$ of these with $U\cap W=0$. If $W+U\ne V$, some simple summand $S$ is not contained in $W+U$. Then $S\cap(W+U)=0$ by simplicity, so $U+S$ is a larger sum disjoint from $W$, a contradiction. Thus $V=W\oplus U$.

We prove the required splitting by [Haar averaging produces invariant complements](../../../../../haar-averaging-produces-invariant-complements.md). The structural input is the [compact real form of a complex semisimple Lie algebra](../../../../../compact-real-form-of-a-complex-semisimple-lie-algebra.md): there is a real semisimple algebra $\mathfrak k$ with $L=\mathfrak k\oplus i\mathfrak k$, whose simply connected integrating Lie group $K$ is compact. This structural fact is independent of the complete-reducibility assertion. One standard construction uses [root vectors](../../../../../root-vector.md) normalized so that $[e_\alpha,e_{-\alpha}]=h_\alpha$, with real structure constants compatible with the involution $e_\alpha\mapsto-e_{-\alpha}$ and $h_\alpha\mapsto-h_\alpha$. The real span

$$
\mathfrak k=\operatorname{span}_{\mathbb R}\{ih_i,\ e_\alpha-e_{-\alpha},\ i(e_\alpha+e_{-\alpha}):\alpha>0\}
$$

is closed under brackets, complexifies to $L$, and has negative-definite [Killing form](../../../../../killing-form.md). The compactness criterion for real semisimple [Lie algebras](../../../../../lie-algebra-split.md) then gives a compact simply connected $K$. Thus this route uses root structure and compact integration, not the theorem being proved.

Restrict $\rho:L\to\operatorname{End}_{\mathbb C}(V)$ to $\mathfrak k$. The [integration of a Lie-algebra representation](../../../../../integration-of-a-lie-algebra-representation.md) gives a representation $R:K\to\operatorname{GL}_{\mathbb C}(V)$, since $K$ is simply connected. Choose any positive-definite [Hermitian inner product](../../../../../hermitian-form.md) $\langle\ ,\ \rangle_0$ and average using normalized [Haar measure](../../../../../haar-measure.md):

$$
\langle v,w\rangle_K=\int_K\langle R(g)v,R(g)w\rangle_0\,d\mu(g).
$$

The integral exists by compactness. It is positive-definite because $R(g)v\ne0$ for $v\ne0$, and it is $K$-invariant by translation invariance of [Haar measure](../../../../../haar-measure.md). Equivalently, every $\rho(a)$ with $a\in\mathfrak k$ is skew-Hermitian for this inner product.

Let $W$ be an $L$-[submodule](../../../../../submodule.md). It is invariant under $\mathfrak k$, hence under the exponentials generating the connected group $K$. For $v\in W^\perp$, $w\in W$ and $g\in K$,

$$
\langle R(g)v,w\rangle_K=\langle v,R(g^{-1})w\rangle_K=0.
$$

Consequently the [orthogonal complement](../../../../../orthogonal-complement.md) $W^\perp$ is $K$-invariant, and differentiation makes it $\mathfrak k$-invariant. It is a complex vector subspace, so it is also invariant under $i\mathfrak k$ and hence under $L$. Therefore $V=W\oplus W^\perp$ as $L$-[modules](../../../../../module-mathematics.md).

Induction on $\dim V$ now expresses $V$ as a finite [direct sum](../../../../../direct-sum.md) of irreducible [submodules](../../../../../submodule.md). **Every finite-dimensional representation of a finite-dimensional complex semisimple [Lie algebra](../../../../../lie-algebra-split.md) is completely reducible.** The compact real form need not be the real form originally used to present $L$; in particular the averaging argument does not require the given presentation to be unitary.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
