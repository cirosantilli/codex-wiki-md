<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We first prove that any two nonzero principal [left ideals](../../../../../left-ideal.md) $Ra$ and $Rb$ intersect nontrivially. Suppose instead that $Ra\cap Rb=0$. The nonzero [left ideals](../../../../../left-ideal.md)

$$
Ra,\quad Rab,\quad Rab^2,\quad\ldots
$$

then form a [direct sum](../../../../../direct-sum.md). Indeed, take a finite relation

$$
\sum_{i=0}^m u_iab^i=0.
$$

It implies

$$
u_0a=-\left(\sum_{i=1}^m u_iab^{i-1}\right)b\in Ra\cap Rb=0.
$$

As $R$ is a [noncommutative domain](../../../../../noncommutative-domain.md) and $a\ne0$, this gives $u_0=0$. Right cancellation of the nonzero element $b$ reduces the remaining relation to one of the same form with one fewer term. Repetition gives $u_1=\cdots=u_m=0$, proving the asserted [direct sum](../../../../../direct-sum.md).

Consequently its finite partial sums give a strictly ascending chain of [left ideals](../../../../../left-ideal.md), contradicting the [ascending chain condition](../../../../../ascending-chain-condition.md) in a [left Noetherian ring](../../../../../left-noetherian-ring.md). Thus $Ra\cap Rb\ne0$ whenever $a,b\ne0$. This is the [left Noetherian domain Ore lemma](../../../../../left-noetherian-domain-ore-lemma.md).

Now take $s\in S=R\setminus\{0\}$ and $r\in R$. If $r=0$, choose $s'=1$ and $r'=0$. Otherwise choose

$$
0\ne z\in Rr\cap Rs,\qquad z=s'r=r's.
$$

Since $z\ne0$, the coefficient $s'$ is nonzero and hence belongs to $S$. This proves the [left Ore set](../../../../../left-ore-set.md) condition in all cases.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the non-commutative rings course of the University of Oxford](../../../../split.md)
6. [Non-commutative rings course of the University of Oxford](../../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
