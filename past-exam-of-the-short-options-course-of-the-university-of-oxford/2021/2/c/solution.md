<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Abelian group criterion for a product of two prime squares](../../../../abelian-group-criterion-for-a-product-of-two-prime-squares.md) applies because $11<19$ and $11\nmid19^2-1=360$. Here its [Sylow theorems](../../../../sylow-theorems.md) proof is especially short:

$$
n_{19}\mid121,\quad n_{19}\equiv1\pmod{19};\qquad n_{11}\mid361,\quad n_{11}\equiv1\pmod{11}.
$$

The candidates for $n_{19}$ are $1,11,121$, of which only $1$ has the required remainder. The candidates for $n_{11}$ are $1,19,361$, again leaving only $1$. Thus both [Sylow subgroups](../../../../sylow-subgroup.md) $P,Q$ are [normal subgroups](../../../../normal-subgroup.md). Their [group commutators](../../../../group-commutator.md) lie in $P\cap Q=\{1\}$, and $PQ=G$, so $G\cong P\times Q$. Both factors are [abelian groups of prime-square order](../../../../abelian-group-of-prime-square-order.md) by (a).

The [Fundamental theorem of finitely generated abelian groups](../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md) gives precisely

$$
\boxed{\begin{gathered}
C_{121}\times C_{361},\qquad C_{121}\times C_{19}\times C_{19},\\
C_{11}\times C_{11}\times C_{361},\qquad C_{11}\times C_{11}\times C_{19}\times C_{19}.
\end{gathered}}
$$

These four [groups](../../../../group-split.md) are pairwise nonisomorphic: their characteristic [Sylow subgroups](../../../../sylow-subgroup.md) differ in whether they contain an element of order $11^2$ or $19^2$. The first is also the [cyclic group](../../../../cyclic-group.md) $C_{43681}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
