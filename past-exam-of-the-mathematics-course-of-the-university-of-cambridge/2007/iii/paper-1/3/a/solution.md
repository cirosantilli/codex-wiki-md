<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $d=\operatorname{diag}(\varpi^{-(n-1)},\ldots,1)$ for the diagonal matrix called $\delta$ in this question. If $v\in V^K$ and $k_i=d^ikd^{-i}\in K_i$, then

$$
\rho(k_i)\rho(d^i)v=\rho(d^i)\rho(k)v=\rho(d^i)v.
$$

Thus $\rho(d^i)$ maps the [fixed-vector space](../../../../../../fixed-vector-space.md) $V^K$ into $V^{K_i}$. Its inverse $\rho(d^{-i})$ gives the reverse map, so

$$
\boxed{V^K\xrightarrow{\ \rho(d^i)\ }V^{K_i}\text{ is an isomorphism}.}
$$

For an upper-unipotent matrix $u$, inverse conjugation changes each entry above the diagonal by

$$
(d^{-i}ud^i)_{rs}=\varpi^{i(s-r)}u_{rs},\qquad r<s.
$$

Every such factor tends to zero as $i\to\infty$. Because $U_0$ is compact, its finitely many coordinate functions are uniformly bounded; because it is open, it contains a neighbourhood of the identity in $U$. Therefore this contraction is uniform on $U_0$ and gives $d^{-i}U_0d^i\subseteq U_0$ for every sufficiently large $i$. The diagonal group commutes with $d$, so

$$
d^{-i}Kd^i=T_0(d^{-i}U_0d^i)\subseteq T_0U_0=K.
$$

Conjugating this inclusion gives $K\subseteq K_i$ for all sufficiently large $i$. This is an eventual inclusion; arbitrary $U_0$ need not give a monotone sequence at every earlier step.

Consequently $V^{K_i}\subseteq V^K$ eventually. Admissibility makes these spaces finite-dimensional, while the isomorphism above makes their dimensions equal. Hence

$$
\boxed{V^{K_i}=V^K\quad\text{for all sufficiently large }i.}
$$

This proves [contraction and admissible fixed spaces](../../../../../../contraction-and-admissible-fixed-spaces.md) by both inclusion and dimension, not by an assumption that conjugate fixed spaces are literally equal from the outset.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
