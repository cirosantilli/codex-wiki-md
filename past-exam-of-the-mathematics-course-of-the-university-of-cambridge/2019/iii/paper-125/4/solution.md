<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Kummer theory](../../../../../kummer-theory.md) begins with the exact sequence

$$
1\longrightarrow\mu_n\longrightarrow\overline K^\times
\xrightarrow{(cdot)^n}\overline K^\times\longrightarrow1.
$$

[Galois cohomology](../../../../../galois-cohomology.md) and Hilbert theorem 90 identify

$$
H^1(K,\mu_n)\cong K^\times/K^{\times n},
$$

so cyclic extensions of exponent dividing $n$ are described by adjoining $n$th roots when $K$ contains $\mu_n$.

For an [elliptic curve](../../../../../elliptic-curve.md) $E/K$, multiplication by $n$ gives the [Kummer exact sequence of an elliptic curve](../../../../../kummer-exact-sequence-of-an-elliptic-curve.md)

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)
\xrightarrow{[n]}E(\overline K)\longrightarrow0.
$$

Its connecting homomorphism is the injective [Kummer map of an elliptic curve](../../../../../kummer-map-of-an-elliptic-curve.md)

$$
E(K)/nE(K)\hookrightarrow H^1(K,E[n]),
\qquad
P\longmapsto(\sigma\mapsto\sigma Q-Q),
$$

where $nQ=P$. Passing to the finite [division field of an elliptic curve](../../../../../division-field-of-an-elliptic-curve.md) $K(E[n])$ makes $E[n]$ constant. Rational functions whose divisors are $n(T)-n(O)$ then express the classes through finitely many elements of $K(E[n])^\times/K(E[n])^{\times n}$.

Let $S$ contain the primes above $n$, the primes of [bad reduction of an elliptic curve](../../../../../bad-reduction-of-an-elliptic-curve.md) and the finitely many primes introduced by these functions. The local theory of good reduction shows that every Kummer class coming from $E(K)$ is unramified outside $S$, so it lies in an [S-unramified power class group](../../../../../s-unramified-power-class-group.md). Such a group is finite: valuations outside $S$ vanish modulo $n$, the [ideal class group](../../../../../ideal-class-group.md) is finite, and the [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) makes the group of $S$-units modulo $n$th powers finite. The kernel created by passing to $K(E[n])$ is finite by finite-group [Galois cohomology](../../../../../galois-cohomology.md). Hence

$$
\boxed{E(K)/nE(K)\text{ is finite}.}
$$

This is the [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../../../kummer-theoretic-proof-of-the-weak-mordell-weil-theorem.md). Combining it with the [height descent lemma](../../../../../height-descent-lemma.md) proves the [Mordell-Weil theorem](../../../../../mordell-weil-group.md): $E(K)$ is a finitely generated abelian group.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 125](../../paper-125-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
