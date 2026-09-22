<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [radical of an ideal](../../../../radical-of-an-ideal.md) $I$ is

$$
\boxed{\sqrt I=\operatorname{rad}(I)=\{a\in R:a^n\in I\text{ for some }n\geq1\}.}
$$

We first establish the properties needed below. If $a^m,b^n\in I$, every term of the [binomial theorem](../../../../binomial-theorem.md) expansion of $(a+b)^{m+n-1}$ contains either $a^m$ or $b^n$, so $a+b\in\sqrt I$. Also $(-a)^m\in I$ and $(ra)^m=r^ma^m\in I$. Thus $\sqrt I$ is an [ideal](../../../../ideal.md). The definition gives $I\subseteq\sqrt I$ and shows that $I\subseteq J$ implies $\sqrt I\subseteq\sqrt J$. Finally, if $a^n\in\sqrt I$, then $(a^n)^m\in I$ for some $m$, so $a\in\sqrt I$. Hence $\sqrt{\sqrt I}=\sqrt I$; in other words, $\sqrt I$ is a [radical ideal](../../../../radical-ideal.md).

We prove the stronger fact that the [radical of an ideal is the intersection of the prime ideals containing it](../../../../radical-of-an-ideal-is-the-intersection-of-the-prime-ideals-containing-it.md):

$$
\sqrt I=\bigcap_{\substack{P\supseteq I\\P\text{ prime}}}P.
$$

If $a\in\sqrt I$ and $P\supseteq I$ is a [prime ideal](../../../../prime-ideal.md), then $a^n\in P$ for some $n$, and repeated application of the definition of a [prime ideal](../../../../prime-ideal.md) gives $a\in P$. This proves one inclusion.

Conversely, fix $a\notin\sqrt I$. The [multiplicatively closed set](../../../../multiplicatively-closed-set.md) $T=\{1,a,a^2,\ldots\}$ is disjoint from $I$. Consider the [ideals](../../../../ideal.md) containing $I$ and disjoint from $T$. This collection is nonempty, and the union of any chain in it is another such [ideal](../../../../ideal.md). By [Zorn's lemma](../../../../zorn-s-lemma.md), there is a maximal member $P$. It is proper because $1\in T$.

To prove that $P$ is a [prime ideal](../../../../prime-ideal.md), suppose $bc\in P$ but $b,c\notin P$. Maximality forces both $P+(b)$ and $P+(c)$ to meet $T$. Thus, for some $u,v\geq0$,

$$
a^u=p+rb,\qquad a^v=q+sc,
\qquad p,q\in P,\quad r,s\in R.
$$

Multiplication gives $a^{u+v}\in P$, since every term lies in $P$, including $rsbc$. This contradicts disjointness from $T$. Therefore $P$ is a [prime ideal](../../../../prime-ideal.md) containing $I$ and avoiding $a$. This proves the other inclusion, including the required [prime ideal avoiding a multiplicative subset](../../../../prime-ideal-avoiding-a-multiplicative-subset.md) argument without using any unproved facts about the [nilradical](../../../../nilradical.md).

If $I=\sqrt I$, the displayed intersection represents $I$ as required. Conversely, an [intersection of ideals](../../../../intersection-of-ideals.md) that are all [prime ideals](../../../../prime-ideal.md) is a [radical ideal](../../../../radical-ideal.md): if $a^n$ belongs to every one of them, then so does $a$. Consequently

$$
\boxed{I=\sqrt I\iff I\text{ is an intersection of prime ideals}.}
$$

The [unit ideal](../../../../unit-ideal.md) $I=R$ is included by interpreting the empty intersection as $R$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
