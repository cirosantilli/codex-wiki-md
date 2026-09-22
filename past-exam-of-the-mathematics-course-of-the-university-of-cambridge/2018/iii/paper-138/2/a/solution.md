<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The roots-of-unity criterion for a [splitting field for finite group representations](../../../../../../splitting-field-for-finite-group-representations.md) says that the assumed $m$th [roots of unity](../../../../../../root-of-unity.md) make $k$ a splitting [field](../../../../../../field.md) for $G$. Fix a multiplicative identification of the group $\mu_m(k)$ with the complex $m$th [roots of unity](../../../../../../root-of-unity.md). For a [p-regular element](../../../../../../p-regular-element.md) $g$, its order divides $m$; the operator $\rho(g)$ is diagonalizable because $X^{|g|}-1$ has distinct roots in $k$. If its [eigenvalues](../../../../../../eigenvalue.md), counted with multiplicity, are $\lambda_1,\ldots,\lambda_d$, define the [Brauer character](../../../../../../brauer-character.md) by

$$
\chi_V(g)=\sum_{i=1}^{d}\widehat\lambda_i,
$$

where hats denote the chosen complex lifts. This defines a [class function](../../../../../../class-function.md) on the [p-regular elements](../../../../../../p-regular-element.md), not on arbitrary elements of $G$.

A [short exact sequence](../../../../../../short-exact-sequence.md) can be represented by block triangular matrices, so the eigenvalue multiset is the union of those on its [submodule](../../../../../../submodule.md) and quotient. Thus [Brauer characters](../../../../../../brauer-character.md) are additive on [short exact sequences](../../../../../../short-exact-sequence.md). If $S_1,\ldots,S_t$ are the simple $kG$-modules, the [Jordan–Hölder theorem](../../../../../../jordan-holder-theorem.md) gives

$$
\chi_V=\sum_{j=1}^{t}[V:S_j]\chi_{S_j}.
$$

We use the standard [Brauer–Nesbitt theorem](../../../../../../brauer-nesbitt-theorem.md) in its character form: over a splitting [field](../../../../../../field.md) the [Brauer characters](../../../../../../brauer-character.md) of the nonisomorphic [simple modules](../../../../../../irreducible-module.md) are linearly independent over $\mathbb C$. Therefore

$$
\boxed{\chi_V=\chi_{V'}\iff[V:S_j]=[V':S_j]\text{ for every }j}.
$$

Both the modular splitting-field criterion and this independence theorem are the representation-theoretic results used here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
