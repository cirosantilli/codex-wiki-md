<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

If $P$ is a prime ideal of the commutative [Artinian ring](../../../../../artinian-ring.md) $R$, then $R/P$ is an Artinian domain. For $0\ne x\in R/P$, the descending chain $(x)\supseteq(x^2)\supseteq\cdots$ stabilizes, so $x^n=x^{n+1}a$ for some $n$; cancellation gives $xa=1$. Thus $R/P$ is a field and $P$ is maximal.

There are only finitely many maximal ideals. Otherwise, distinct maximal ideals $P_i$ are pairwise comaximal and their finite products give the strictly descending chain

$$
P_1\supsetneq P_1P_2\supsetneq P_1P_2P_3\supsetneq\cdots,
$$

contradicting the Artinian condition. This proves the statement about the [prime ideals of a commutative Artinian ring](../../../../../prime-ideals-of-a-commutative-artinian-ring.md).

The [nilradical](../../../../../nilradical.md) $N$ is the ideal of all nilpotent elements, equivalently the intersection of all prime ideals. Its powers stabilize, say $N^r=N^{r+1}=I$. If $I\ne0$, choose an ideal $J$ minimal subject to $IJ\ne0$, then choose $x\in J$ with $Ix\ne0$. Since $I^2=I$, minimality gives $Rx=Ix$, so $x=ax$ for some $a\in I$. But $a$ is nilpotent, hence $1-a$ is a unit, contradicting $(1-a)x=0$. Therefore the [nilradical of a commutative Artinian ring](../../../../../nilradical-of-a-commutative-artinian-ring.md) is nilpotent.

If the maximal ideals are $P_1,\ldots,P_s$, the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives

$$
R/N\cong\prod_{i=1}^sR/P_i,
$$

a finite product of fields. Each layer $N^j/N^{j+1}$ is an Artinian module over this product and therefore finite-dimensional. Since $N$ is nilpotent, these finitely many layers show that every ideal of $R$ is finitely generated. This proves the [Artinian commutative ring is Noetherian theorem](../../../../../artinian-commutative-ring-is-noetherian-theorem.md).

Now assume $R$ is local with maximal ideal $P$ and $\dim_{R/P}P/P^2=1$. The [Nakayama lemma](../../../../../nakayama-lemma.md) gives $P=(x)$. Since $P$ is nilpotent, its powers form a finite chain ending in zero. For a nonzero ideal $J$, choose the largest $r$ with $J\subseteq(x^r)$ and take $y\in J\setminus(x^{r+1})$. Write $y=x^ru$; then $u\notin P$, so $u$ is a unit. Hence

$$
J\subseteq(x^r)=(y)\subseteq J,
$$

and **every ideal of $R$ is principal**.

Finally, the [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) says that a finite-dimensional semisimple $k$-algebra has the form

$$
\boxed{T\cong\prod_{i=1}^sM_{n_i}(D_i),}
$$

where each $D_i$ is a finite-dimensional [division ring](../../../../../division-ring.md) over $k$; the factors are unique up to permutation and isomorphism. By the assumed complete reducibility, write the right regular module as

$$
T_T\cong\bigoplus_{i=1}^sS_i^{n_i}
$$

with pairwise nonisomorphic simple right modules $S_i$. The [Schur lemma](../../../../../schur-s-lemma.md) says that $D_i=\operatorname{End}_T(S_i)$ is a division ring and that homomorphisms between distinct $S_i$ vanish. Left multiplication and the [endomorphism ring](../../../../../endomorphism-ring.md) of the displayed direct sum therefore give

$$
T\cong\operatorname{End}_T(T_T)
\cong\prod_iM_{n_i}(D_i).
$$

Conversely, the regular module of $M_n(D)$ is a direct sum of $n$ simple column modules, proving that every algebra on the right is semisimple. Uniqueness follows from uniqueness of the simple summands and their multiplicities.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 148](../../paper-148-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
