<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Jacobson radical](../../../../../jacobson-radical.md) $J=J(R)$ is the intersection of all maximal right ideals, equivalently the largest ideal annihilating every simple right module. The [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) gives

$$
\boxed{R/J\simeq\prod_{a=1}^tM_{n_a}(k)}
$$

because $k$ is algebraically closed.

The descending chain $J\supseteq J^2\supseteq\cdots$ stabilizes since $R$ is finite-dimensional. If $J^m=J^{m+1}$, [Nakayama lemma](../../../../../nakayama-lemma.md) applied to the finite right module $J^m$ gives $J^m=0$. Thus $J$ is nilpotent.

For $f\in\operatorname{End}_R(P_i)$, the [Fitting lemma](../../../../../fitting-lemma.md) gives

$$
P_i=\ker f^n\oplus\operatorname{im}f^n
$$

for large $n$. Indecomposability makes one summand zero, so $f$ is either invertible or nilpotent. In the latter case $1-f$ is invertible. This is the criterion that $\operatorname{End}_R(P_i)$ is a [local ring](../../../../../local-ring.md).

Let $M=\bigoplus_iP_i$. Reduction modulo $MJ$ defines

$$
\theta:\operatorname{End}_R(M)\longrightarrow\operatorname{End}_R(M/MJ).
$$

Since $M/MJ=\bigoplus_iS_i$ and the $S_i$ are pairwise nonisomorphic simples,

$$
\operatorname{End}_R(M/MJ)\simeq\prod_i\operatorname{End}_R(S_i)\simeq k^n
$$

by [Schur lemma](../../../../../schur-s-lemma.md). Arbitrary scalars on the direct summands lift to scalar identity maps on the $P_i$, so $\theta$ is surjective.

If $f\in\ker\theta$, then $f(M)\subseteq MJ$. A product of $r$ such maps sends $M$ into $MJ^r$, so $\ker\theta$ is nilpotent. A nilpotent ideal lies in the Jacobson radical, while the semisimplicity of the quotient $k^n$ gives the reverse inclusion. Hence

$$
\boxed{J(\operatorname{End}_R(M))=\ker\theta,\qquad
\operatorname{End}_R(M)/J\simeq k^n.}
$$

This is exactly the definition of a [basic algebra](../../../../../basic-algebra.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
