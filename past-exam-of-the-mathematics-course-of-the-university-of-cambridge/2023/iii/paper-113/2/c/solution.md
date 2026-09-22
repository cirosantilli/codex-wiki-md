<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Cartier divisor](../../../../../../cartier-divisor-split.md) on an integral scheme is an open cover $(U_i)$ together with nonzero rational functions $f_i$ such that every ratio $f_i/f_j$ is a regular unit on $U_i\cap U_j$.

Every [prime Weil divisor](../../../../../../prime-weil-divisor.md) on $\mathbb P_k^n$ is cut out by an irreducible homogeneous polynomial because the [polynomial ring](../../../../../../polynomial-ring.md) $k[x_0,\ldots,x_n]$ is a [unique factorization domain](../../../../../../unique-factorization-domain.md). Hence any [Weil divisor](../../../../../../weil-divisor.md) can be represented by a homogeneous rational expression

$$
F=\prod_jF_j^{m_j}
$$

of some total degree $d$. On the standard chart $U_i=D_+(x_i)$, put $f_i=F/x_i^d$. This is a degree-zero rational function, and on $U_i\cap U_j$,

$$
\frac{f_i}{f_j}=\left(\frac{x_j}{x_i}\right)^d
$$

is a regular unit. These local equations form a Cartier divisor whose associated Weil divisor is the original one.

Now put $P=X\times\mathbb P^n$ and let $H=X\times\mathbb P^{n-1}$ be the [hyperplane divisor](../../../../../../hyperplane-divisor.md) at infinity. Its complement is $X\times\mathbb A^n$. Iterating the given invariance under multiplication by $\mathbb A^1$ gives

$$
\operatorname{Cl}(X\times\mathbb A^n)\cong\operatorname{Cl}(X).
$$

The [localization sequence for the divisor class group](../../../../../../localization-sequence-for-the-divisor-class-group.md) shows that every class on $P$ is a pullback of a class on $X$ plus an integer multiple of $[H]$. Restriction to the generic fiber $\mathbb P^n_{K(X)}$ kills pullbacks from $X$ and sends $[H]$ to the generator of $\operatorname{Cl}(\mathbb P^n_{K(X)})\cong\mathbb Z$. Therefore the sum is direct, proving

$$
\operatorname{Cl}(X\times\mathbb P^n)
\cong\operatorname{Cl}(X)\oplus\mathbb Z.
$$

This is the [divisor class group of a projective-space bundle with trivial vector bundle](../../../../../../divisor-class-group-of-a-projective-space-bundle-with-trivial-vector-bundle.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
