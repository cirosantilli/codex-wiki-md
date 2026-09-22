<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $V=\mathbb C^n$ and $m\geq0$. Identify the [symmetric power](../../../../../symmetric-power.md) $\operatorname{Sym}^mV$ with the degree-$m$ part of the symmetric algebra on the basis vectors $e_1,\ldots,e_n$, using formal variables $x_i$ for these vectors. Its monomial basis is

$$
x^a=x_1^{a_1}\cdots x_n^{a_n},\qquad a_i\geq0,\qquad\sum_i a_i=m.
$$

The diagonal [maximal torus](../../../../../maximal-torus.md) of the [unitary group](../../../../../unitary-group.md) acts on this monomial by the character $z_1^{a_1}\cdots z_n^{a_n}$. Distinct tuples give distinct characters, so each [weight space](../../../../../weight-space.md) is one-dimensional.

Suppose $M$ is a nonzero invariant complex subspace. For a nonzero vector $w\in M$, select a monomial with nonzero coefficient and extract it by torus averaging:

$$
\int_T z_1^{-a_1}\cdots z_n^{-a_n}\,t\cdot w\,dt.
$$

[Fourier orthogonality](../../../../../fourier-orthogonality.md) makes this a nonzero scalar multiple of $x^a$. It belongs to $M$, so $M$ contains a monomial.

Differentiating the [unitary group](../../../../../unitary-group.md) action makes $M$ invariant under $\mathfrak u(n)$ and hence under its complexification $\mathfrak{gl}_n(\mathbb C)$. The matrix unit $E_{ij}$ replaces an occurrence of $e_j$ by $e_i$, so its action on the symmetric algebra is

$$
E_{ij}\cdot x^a=x_i\partial_{x_j}x^a
=a_jx^{a+e_i-e_j}.
$$

Whenever $a_j>0$, this transfers one unit of degree from coordinate $j$ to coordinate $i$ with a nonzero coefficient. Starting with any monomial, such transfers can produce every other tuple of nonnegative integers summing to $m$. Thus $M$ contains every monomial and equals $\operatorname{Sym}^mV$.

Consequently

$$
\boxed{\operatorname{Sym}^m\mathbb C^n\text{ is irreducible for every }m\geq0.}
$$

For $m=0$ this is the one-dimensional trivial representation, and for $n=1$ every symmetric power is also one-dimensional. This [weight-transfer proof of irreducibility of symmetric powers](../../../../../weight-transfer-proof-of-irreducibility-of-symmetric-powers.md) uses neither the [Weyl character formula](../../../../../weyl-character-formula.md) nor the [Weyl dimension formula](../../../../../weyl-dimension-formula.md), so no unproved dimension formula enters the argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
