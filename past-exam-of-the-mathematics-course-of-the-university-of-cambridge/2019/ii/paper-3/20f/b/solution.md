<h1 id="20f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inclusion and passage to the quotient give a [short exact sequence of chain complexes](../../../../../../short-exact-sequence-of-chain-complexes.md)

$$
0\longrightarrow C_\bullet(L)
\xrightarrow{i}C_\bullet(K)
\xrightarrow{q}C_\bullet(K,L)
\longrightarrow0.
$$

Define the [connecting homomorphism](../../../../../../connecting-homomorphism.md) as follows. If $[c]\in H_k(K,L)$, then $\bar\partial[c]=0$, so $\partial c\in C_{k-1}(L)$. Since $\partial^2c=0$, it is a [chain cycle](../../../../../../chain-cycle.md) in $L$, and we set

$$
\delta[c]=[\partial c]\in H_{k-1}(L).
$$

Changing $c$ by a relative boundary or a chain in $L$ changes $\partial c$ by a boundary in $L$, so $\delta$ is well defined.

The resulting sequence is

$$
\boxed{
\cdots\longrightarrow H_k(L)
\xrightarrow{i_*}H_k(K)
\xrightarrow{q_*}H_k(K,L)
\xrightarrow{\delta}H_{k-1}(L)
\xrightarrow{i_*}H_{k-1}(K)
\longrightarrow\cdots.}
$$

We verify exactness directly. If a cycle of $K$ maps to zero in the relative homology, it differs from a boundary by a cycle in $L$, so it lies in $\operatorname{im}i_*$. If a relative cycle $[c]$ satisfies $\delta[c]=0$, then $\partial c=\partial\ell$ for some $\ell\in C_k(L)$; hence $c-\ell$ is a cycle in $K$ mapping to $[c]$. Finally, if a cycle $z\in C_{k-1}(L)$ becomes a boundary in $K$, say $z=\partial c$, then $[c]$ is a relative cycle with $\delta[c]=[z]$. The reverse containments follow immediately from consecutive composites being zero. This proves the [long exact sequence in relative homology](../../../../../../long-exact-sequence-in-relative-homology.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
