<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [bounded-size transversal kernel](../../../../../../bounded-size-transversal-kernel.md) gives a [finite intersection witness for cross-intersecting families](../../../../../../finite-intersection-witness-for-cross-intersecting-families.md), even when the two [set families](../../../../../../set-family.md) are infinite. We first prove the kernel statement: for any [set family](../../../../../../set-family.md) $\mathcal F$ whose members have size at most $r$, and any integer $s\geq0$, there is a finite [subset](../../../../../../subset.md) $\mathcal F_0\subseteq\mathcal F$ with

$$
|\mathcal F_0|\leq M(r,s):=\sum_{j=0}^{s}r^j
$$

such that every [set](../../../../../../set-split.md) $H$ of size at most $s$ is a [hitting set](../../../../../../hitting-set.md) for $\mathcal F_0$ if and only if it is a [hitting set](../../../../../../hitting-set.md) for $\mathcal F$.

Use [mathematical induction](../../../../../../mathematical-induction.md) on $s$. If $\mathcal F$ is empty, take $\mathcal F_0=\varnothing$. For $s=0$ and nonempty $\mathcal F$, choose any one member: the only possible $H$ is empty and is a [hitting set](../../../../../../hitting-set.md) for neither family. For the induction step, choose $A_0\in\mathcal F$. For each $x\in A_0$ apply the inductive statement to

$$
\mathcal F_x=\{A\in\mathcal F:x\notin A\}
$$

with parameter $s-1$, obtaining $\mathcal F_{x,0}$. Put $\mathcal F_0=\{A_0\}\cup\bigcup_{x\in A_0}\mathcal F_{x,0}$. Its size is at most $1+rM(r,s-1)=M(r,s)$. If $H$ is a [hitting set](../../../../../../hitting-set.md) for $\mathcal F_0$, choose $x\in H\cap A_0$. Every member of $\mathcal F_{x,0}$ avoids $x$, so $H\setminus\{x\}$ is a [hitting set](../../../../../../hitting-set.md) for $\mathcal F_{x,0}$ and hence for $\mathcal F_x$. Members of $\mathcal F$ containing $x$ already meet $H$. Thus $H$ is a [hitting set](../../../../../../hitting-set.md) for all of $\mathcal F$. The reverse implication follows from inclusion. If $A_0=\varnothing$, no $H$ is a [hitting set](../../../../../../hitting-set.md) for either family, so the implication remains valid. This finite branching proof never assumes $\mathcal F$ is finite.

Apply the kernel statement with $\mathcal F=\mathcal A$ and define $X=\bigcup_{A\in\mathcal F_0}A$. For each $B\in\mathcal B$, the [cross-intersecting family](../../../../../../cross-intersecting-family.md) condition ensures that $B\cap X$ meets every member of $\mathcal F_0$, since these members lie inside $X$. As $|B\cap X|\leq s$, it therefore meets every $A\in\mathcal A$. We obtain

$$
\boxed{A\cap B\cap X\ne\varnothing\quad\text{for every }A\in\mathcal A,\ B\in\mathcal B,\qquad |X|\leq r\sum_{j=0}^{s}r^j.}
$$

In particular, a positive-integer-valued choice valid whether or not $0\in\mathbb N$ is

$$
\boxed{f(r,s)=1+r\sum_{j=0}^{s}r^j.}
$$

Here the constant term of the sum is $1$, including when $r=0$. If either [set family](../../../../../../set-family.md) is empty, $X=\varnothing$ suffices. If both are nonempty, the [cross-intersecting family](../../../../../../cross-intersecting-family.md) condition rules out $r=0$ or $s=0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
