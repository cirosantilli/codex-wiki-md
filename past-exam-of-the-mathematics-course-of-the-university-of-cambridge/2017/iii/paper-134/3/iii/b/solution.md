<h1 id="3/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an [ample Cartier divisor](../../../../../../../ample-cartier-divisor.md) $H$. Put initially $A=\delta H$, $A'=tH$ for small positive real $\delta,t$. Since $D$ is [nef](../../../../../../../nef-line-bundle.md), the [nef-plus-ample ampleness lemma](../../../../../../../nef-plus-ample-ampleness-lemma.md) makes $D+tH$ [ample](../../../../../../../ample-line-bundle.md). The polynomial

$$
P(\delta,t)=(D+tH)^n-n(D+tH)^{n-1}\cdot((\delta+t)H)
$$

has $P(0,0)=D^n\cdot[X]>0$. Thus the desired strict inequality holds when $\delta,t$ are sufficiently small and positive.

We must also arrange rationality of the two specified classes; $D$ itself need not be rational. Choose rational [ample](../../../../../../../ample-line-bundle.md) classes $B$ and $C$ sufficiently near $D+tH$ and $(\delta+t)H$, and define

$$
A'=B-D,\qquad A=C-A'=C-B+D.
$$

Then $A'$ is close to $tH$ and $A$ is close to $\delta H$, so both are [ample real divisors](../../../../../../../ample-real-divisor.md) by openness of the [ample cone](../../../../../../../ample-cone.md). Also $D+A'=B$ and $A+A'=C$ are rational and [ample](../../../../../../../ample-line-bundle.md). Continuity preserves the strict inequality, giving

$$
\boxed{B^n>nB^{n-1}\cdot C,\qquad D-A=B-C.}
$$

Here is the needed [algebraic Morse inequality for ample divisors](../../../../../../../algebraic-morse-inequality-for-ample-divisors.md), with its section-count proof. Choose rational [Cartier divisor](../../../../../../../cartier-divisor-split.md) representatives of $B,C$ and a common positive integer $q$ making $qB,qC$ [very ample](../../../../../../../very-ample-line-bundle.md) integral [Cartier divisors](../../../../../../../cartier-divisor-split.md). For the section-count argument rename these scaled representatives $B,C$; undoing this scaling restricts section indices to sufficiently divisible multiples and leaves bigness unchanged. Choose an effective [Cartier divisor](../../../../../../../cartier-divisor-split.md) $G\in|C|$ by taking a defining section that avoids the [associated points](../../../../../../../associated-point-of-a-coherent-sheaf.md) of $\mathcal O_X$. Repeated [divisor restriction exact sequences](../../../../../../../divisor-restriction-exact-sequence.md) give

$$
h^0(X,m(B-C))\ge h^0(X,mB)-\sum_{j=0}^{m-1}h^0(G,\mathcal O_G(mB-jC)).
$$

Because $C$ is [very ample](../../../../../../../very-ample-line-bundle.md), for each $j$ a section of $jC$ avoiding the finitely many [associated points](../../../../../../../associated-point-of-a-coherent-sheaf.md) of $\mathcal O_G$ gives an injection into $\mathcal O_G(mB)$. Thus every summand is at most $h^0(G,\mathcal O_G(mB))$. By [Serre vanishing](../../../../../../../serre-vanishing.md) and [asymptotic Riemann–Roch](../../../../../../../asymptotic-riemann-roch.md) for the [ample](../../../../../../../ample-line-bundle.md) $B$,

$$
h^0(X,m(B-C))\ge\frac{B^n-nB^{n-1}\cdot C}{n!}m^n+O(m^{n-1}).
$$

For $n=1$, the restriction term is the constant length of $G$, giving the same formula directly. The positive coefficient proves that $B-C$, hence $D-A$, is big. Scaling back preserves bigness, so

$$
\boxed{D-A\text{ is big}.}
$$

For a general [projective scheme](../../../../../../../projective-scheme.md), enforce the same strict inequality separately on each positive-dimensional reduced irreducible component $V_j$, using its own dimension $n_j$. At $(\delta,t)=(0,0)$ every such expression equals the positive number $D^{n_j}\cdot[V_j]$. Finitely many conditions are preserved by one sufficiently small choice and one sufficiently close rational approximation on $N^1(X)_{\mathbb R}$. The top-dimensional inequalities imply the printed inequality for $[X]$ with its positive generic multiplicities; the section proof on each component makes $D-A$ componentwise big. This avoids inferring bigness on every component from just a positive sum. The displayed inequality is used for $n\ge1$. For $n=0$, its literal $n-1$ intersection power is undefined; handle this vacuous positivity case separately. Every [line bundle](../../../../../../../line-bundle.md) is [ample](../../../../../../../ample-line-bundle.md), all [numerical classes](../../../../../../../real-numerical-divisor-classes.md) are zero, and the componentwise bigness convention makes the conclusions automatic.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [3](../../../3.md)
4. [Paper 134](../../../../paper-134-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
