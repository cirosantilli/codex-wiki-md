<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [prime radical of a noncommutative ring](../../../../../prime-radical-of-a-noncommutative-ring.md) is $N(R)=\bigcap_P P$, with $P$ ranging over all [prime ideals of a noncommutative ring](../../../../../prime-ideal-of-a-noncommutative-ring.md). Here primeness means that for two-sided [ideals](../../../../../ideal.md) $A,B$, $AB\subseteq P$ implies $A\subseteq P$ or $B\subseteq P$. A [minimal prime over an ideal](../../../../../minimal-prime-over-an-ideal.md) $I$ is a [prime ideal](../../../../../prime-ideal.md) containing $I$ with no strictly smaller [prime ideal](../../../../../prime-ideal.md) containing $I$.

The [ascending chain condition](../../../../../ascending-chain-condition.md) on [left ideals](../../../../../left-ideal.md) also applies to two-sided [ideals](../../../../../ideal.md). We first prove by [Noetherian induction](../../../../../noetherian-induction.md) that every proper $I$ contains a finite product of [prime ideals](../../../../../prime-ideal.md), each containing $I$. If there were counterexamples, choose a maximal one. It is not prime, so there are strictly larger two-sided [ideals](../../../../../ideal.md) $A,B$ with $AB\subseteq I$. Neither is a counterexample; products of [prime ideals](../../../../../prime-ideal.md) contained in $A$ and in $B$ then concatenate to a product contained in $I$, a contradiction.

Write $P_1\cdots P_t\subseteq I\subseteq P_j$. Every [prime ideal](../../../../../prime-ideal.md) $P$ over $I$ contains at least one $P_j$, by primeness. The inclusion-minimal members of the finite list $P_j$ are therefore precisely the [minimal primes over an ideal](../../../../../minimal-prime-over-an-ideal.md) $I$: any smaller prime over $I$ would contain a member of that same list. Consequently there are finitely many. Replacing each factor $P_j$ by a minimal prime contained in it gives

$$
Q_1Q_2\cdots Q_t\subseteq I
$$

with each $Q_j$ minimal over $I$. Repeated factors may be necessary; in $k[\varepsilon]/(\varepsilon^m)$ the sole minimal prime $(\varepsilon)$ requires its $m$th power to reach zero.

Apply this to $I=0$. Since $N(R)\subseteq Q_j$ for every $j$,

$$
\boxed{N(R)^t\subseteq Q_1\cdots Q_t=0}.
$$

Thus the [prime radical](../../../../../prime-radical-of-a-noncommutative-ring.md) is a [nilpotent ideal](../../../../../nilpotent-ideal.md), as in [finite minimal primes and nilpotent prime radical](../../../../../finite-minimal-primes-and-nilpotent-prime-radical.md).

Now assume $R$ is commutative. A [prime ideal](../../../../../prime-ideal.md) $P$ is an [associated prime of a module](../../../../../associated-prime-of-a-module.md) $M$ when $P=\operatorname{Ann}_R(m)$ for some $0\ne m\in M$. Every nonzero [module](../../../../../module-mathematics.md) over $R$ has an associated prime: the [ascending chain condition](../../../../../ascending-chain-condition.md) gives a maximal annihilator of a nonzero element, and [maximal annihilator of a module element is prime](../../../../../maximal-annihilator-of-a-module-element-is-prime.md).

Since the given $M$ is a [Noetherian module](../../../../../noetherian-module.md), repeatedly choosing such a cyclic [submodule](../../../../../submodule.md) in the next quotient yields a finite [prime filtration](../../../../../prime-filtration.md)

$$
0=M_0\subsetneq M_1\subsetneq\cdots\subsetneq M_s=M,
\qquad M_i/M_{i-1}\cong R/P_i.
$$

The process terminates by the [ascending chain condition](../../../../../ascending-chain-condition.md). In a [short exact sequence](../../../../../short-exact-sequence.md) $0\to U\to M\to W\to0$, one has $\operatorname{Ass}(M)\subseteq\operatorname{Ass}(U)\cup\operatorname{Ass}(W)$. Indeed, if $P=\operatorname{Ann}(m)$ and $Rm\cap U=0$, the image of $m$ in $W$ still has annihilator $P$. Otherwise choose $0\ne am\in U$; then $a\notin P$, and primeness gives $\operatorname{Ann}(am)=P$. As $\operatorname{Ass}(R/P_i)=\{P_i\}$, induction along the [prime filtration](../../../../../prime-filtration.md) proves

$$
\boxed{\operatorname{Ass}_R(M)\subseteq\{P_1,\ldots,P_s\}}.
$$

In particular there are only finitely many [associated primes of a module](../../../../../associated-prime-of-a-module.md).

Finally let $P$ be a [minimal prime ideal](../../../../../minimal-prime-ideal.md) of $R$. Its [localization at a prime ideal](../../../../../localization-at-a-prime-ideal.md) $R_P$ has exactly one prime, its [maximal ideal](../../../../../maximal-ideal.md) $PR_P$. The preceding nilpotence result makes this maximal ideal nilpotent. Choose $0\ne y\in R_P$ annihilated by $PR_P$, for example a nonzero element in its last nonzero power, or $1$ if $PR_P=0$. Since elements outside the maximal ideal are [units](../../../../../unit-in-a-ring.md), $\operatorname{Ann}_{R_P}(y)=PR_P$.

Write $y=r/s$. The element $r/1$ is nonzero and also has annihilator $PR_P$. Generate $P$ by $p_1,\ldots,p_\ell$. For each $i$, choose $u_i\notin P$ with $u_ip_ir=0$, and put $u=\prod_i u_i$. Then $m=ur$ remains nonzero after localization, while $Pm=0$. If $am=0$, localization forces $a/1\in PR_P$, and hence $a\in P$. Therefore $\operatorname{Ann}_R(m)=P$. This proves that [minimal primes are associated primes](../../../../../minimal-primes-are-associated-primes.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
