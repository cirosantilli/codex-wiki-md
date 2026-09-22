<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

[Dedekind factorization theorem](../../../../dedekind-factorization-theorem.md) states that if $K=\mathbb Q(\theta)$ with integral $\theta$ and $p$ does not divide $[\mathcal O_K:\mathbb Z[\theta]]$, then a factorization $\overline f=\prod_i\overline f_i^{e_i}$ of its [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) into distinct monic [irreducible polynomials](../../../../irreducible-polynomial.md) over $\mathbb F_p$ gives

$$
p\mathcal O_K=\prod_iP_i^{e_i},\qquad
P_i=(p,f_i(\theta)),\qquad N(P_i)=p^{\deg f_i}.
$$

The factors are distinct [prime ideals](../../../../prime-ideal.md); the residue degrees and ramification indices satisfy $\sum_i e_i\deg f_i=[K:\mathbb Q]$. Unique [prime ideal factorization](../../../../prime-ideal-factorization.md) holds in the [ring of integers](../../../../ring-of-integers.md).

For a [square-free integer](../../../../square-free-integer.md) $d\equiv1\pmod4$, $\mathcal O_K=\mathbb Z[\sqrt{-d}]$, so the index condition is automatic. If $p_i\mid d$, the [polynomial](../../../../polynomial-split.md) $X^2+d$ reduces to $X^2$ modulo $p_i$. Hence

$$
p_i\mathcal O_K=P_i^2,\qquad P_i=(p_i,\sqrt{-d}),\qquad N(P_i)=p_i.
$$

Therefore $d\mathcal O_K=(\prod_iP_i)^2=(\sqrt{-d})^2$. By unique [prime ideal factorization](../../../../prime-ideal-factorization.md), $\prod_iP_i=(\sqrt{-d})$.

Let $S$ be a nonempty proper subset and put $m=\prod_{i\in S}p_i$. For $d>1$, $1<m<d$ and $m$ is a [square-free integer](../../../../square-free-integer.md). If $\prod_{i\in S}P_i=(u+v\sqrt{-d})$, its [ideal norm](../../../../ideal-norm.md) gives

$$
m=u^2+dv^2.
$$

The inequality $m<d$ forces $v=0$, leaving $m=u^2$, impossible for a [square-free integer](../../../../square-free-integer.md) greater than one. Thus every such subproduct is nonprincipal.

These are [ramified prime classes for discriminant minus four d](../../../../ramified-prime-classes-for-discriminant-minus-four-d.md). The [ideal classes](../../../../ideal-class.md) $[P_i]$ have order dividing two. Their product is the identity, and the preceding proof rules out every other nonempty subset relation. The [homomorphism](../../../../homomorphism.md) $\mathbb F_2^k\to\operatorname{Cl}(K)$ defined by these classes consequently has kernel exactly $\{0,(1,\ldots,1)\}$. Its image is therefore

$$
\boxed{C_2^{\,k-1}.}
$$

The boundary case $d=1$ has $k=0$ and makes the printed exponent $k-1$ meaningless; its [field](../../../../field.md) is $\mathbb Q(i)$ with trivial [ideal class group](../../../../ideal-class-group.md). The subgroup statement is understood for $d>1$, while the prime-factor and proper-subset statements are empty for $d=1$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
