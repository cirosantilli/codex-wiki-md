<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [exchange condition for a Coxeter group](../../../../../../exchange-condition-for-a-coxeter-group.md) says that if $w=s_1\cdots s_n$ is reduced and $s$ is simple with $\ell(ws)<\ell(w)$, then

$$
ws=s_1\cdots\widehat{s_j}\cdots s_n
$$

for some $j$. The [Matsumoto theorem](../../../../../../matsumoto-theorem.md) says that any two reduced expressions for the same element are connected by [braid moves](../../../../../../braid-relation-in-a-coxeter-group.md). Together they imply the [Tits word reduction theorem](../../../../../../tits-word-reduction-theorem.md): a nonreduced word can be transformed by braid moves until two equal adjacent generators can be cancelled.

For the displayed four-armed graph, call the central generator $s$ and the leaves $a,b,c,d$. Different leaves commute, while each leaf $t$ satisfies $sts=tst$. Consider the word

$$
u_N=(s\,a\,b\,s\,c\,d)^N.
$$

Between successive occurrences of $s$, the intervening leaf sets alternate between $\{a,b\}$ and $\{c,d\}$. Commuting the two leaves in one block never puts the same leaf on both sides of an $s$, so no length-three braid $tst\leftrightarrow sts$ is ever available. The only possible braid moves are those leaf commutations, and they cannot create adjacent equal letters. Tits reduction therefore shows that $u_N$ is reduced. Since $\ell(u_N)=6N$ is unbounded, the group is infinite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
