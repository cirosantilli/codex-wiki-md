<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For each $j\geq0$, the [elementary abelian group](../../../../../../elementary-abelian-group.md) $P_j/P_{j+1}$ is spanned by the images of $a_i^{p^j}$. We construct exponents $e_i$ so that $g$ equals the ordered product $a_1^{e_1}\cdots a_n^{e_n}$ to successively greater precision. Suppose this product agrees with $g$ modulo $P_j$; initially this is automatic for $j=0$. Its error modulo $P_{j+1}$ can be expressed using the images of $a_i^{p^j}$. Add the corresponding digits $p^jt_i$ to the exponents $e_i$. Since $[P_j,G]\subseteq P_{j+1}$, moving each new factor $a_i^{p^jt_i}$ past the other factors changes nothing modulo $P_{j+1}$. The new ordered product therefore agrees with $g$ modulo $P_{j+1}$. Termination of the [lower p-series](../../../../../../lower-p-series.md) proves

$$
\boxed{G=\langle a_1\rangle\langle a_2\rangle\cdots\langle a_n\rangle.}
$$

No uniqueness of this factorization is asserted for a redundant generating tuple.

**The printed converse is false without an additional condition.** For any odd $p$, take the [Heisenberg group](../../../../../../heisenberg-group.md) $G=\operatorname{UT}_3(\mathbb F_p)$ with

$$
x=I+E_{12},\quad y=I+E_{23},\quad z=I+E_{13}=[x,y].
$$

Every element is uniquely $x^ay^bz^c$, with $a,b,c\in\mathbb F_p$, so $G$ is a product of three [cyclic subgroups](../../../../../../cyclic-subgroup.md). For $A$ strictly upper triangular, $A^3=0$ and

$$
(I+A)^p=I+pA+\binom p2A^2=I
$$

in characteristic $p$, including $p=3$. Therefore $G^p=1$, whereas $[G,G]=\langle z\rangle\ne1$. This [finite p-group](../../../../../../finite-p-group.md) is not powerful, disproving the literal request in the authoritative PDF.

A precise nearby correction is the [minimal cyclic factorization criterion for powerful p-groups](../../../../../../minimal-cyclic-factorization-criterion-for-powerful-p-groups.md): require a product of $d(G)$ cyclic subgroups, where $d(G)$ is the minimal generator number. To prove it, put $d=d(G)$ and $H=G/G^p$. The quotient has exponent $p$ and still has minimal generator number $d$, because $G^p\subseteq\Phi(G)$. Each cyclic factor has image of order at most $p$, so $|H|\leq p^d$. But $|H/\Phi(H)|=p^d$ by the [Burnside basis theorem](../../../../../../burnside-basis-theorem.md). Consequently $\Phi(H)=1$, $H$ is an [elementary abelian group](../../../../../../elementary-abelian-group.md), and $[G,G]\subseteq G^p$. **A product of exactly $d(G)$ cyclic subgroups is powerful.** A direct product of cyclic groups is also powerful, since it is abelian; neither stronger hypothesis appears in the printed converse.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
