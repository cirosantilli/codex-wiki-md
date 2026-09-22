<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [essential right ideal](../../../../../essential-right-ideal.md) intersects every nonzero [right ideal](../../../../../right-ideal.md) nontrivially. A [regular element of a ring](../../../../../regular-element-of-a-ring.md) is a two-sided [non-zero-divisor](../../../../../non-zero-divisor.md): both $cr=0$ and $rc=0$ imply $r=0$. Writing $S$ for the set of these elements, the [classical right ring of quotients](../../../../../classical-right-ring-of-quotients.md) is a [ring](../../../../../ring.md) $Q$ containing $R$, with every $s\in S$ invertible and every element of $Q$ expressible as $as^{-1}$.

[Goldie theorem](../../../../../goldie-s-theorem.md) states that a [semiprime ring](../../../../../semiprime-ring.md) has a semisimple Artinian [classical right ring of quotients](../../../../../classical-right-ring-of-quotients.md) if and only if it is a [right Goldie ring](../../../../../right-goldie-ring.md): it satisfies the [ascending chain condition](../../../../../ascending-chain-condition.md) on right annihilators and has finite [uniform dimension](../../../../../uniform-dimension.md). In particular, every [semiprime ring](../../../../../semiprime-ring.md) that is a [right Noetherian ring](../../../../../right-noetherian-ring.md) satisfies the theorem. We prove the requested case directly using the supplied assumption about [essential right ideals](../../../../../essential-right-ideal.md).

First let $c\in S$. If a nonzero [right ideal](../../../../../right-ideal.md) $B$ had $B\cap cR=0$, the sum

$$
B+cB+c^2B+\cdots
$$

would be direct. Indeed, a finite relation $b_0+cb_1+\cdots+c^mb_m=0$ gives $b_0\in B\cap cR$, hence $b_0=0$; cancellation of $c$ repeats the argument. Each $c^jB$ is a nonzero [right ideal](../../../../../right-ideal.md), so the partial sums form a strictly ascending chain. This contradicts [right Noetherianity](../../../../../right-noetherian-ring.md). Thus [a regular principal right ideal in a right Noetherian ring is essential](../../../../../a-regular-principal-right-ideal-in-a-right-noetherian-ring-is-essential.md), and every [right ideal](../../../../../right-ideal.md) containing $c$ is essential.

For $r\in R$ and $c\in S$, put

$$
E=\{x\in R:rx\in cR\}.
$$

This is an [essential right ideal](../../../../../essential-right-ideal.md). To check this, take a nonzero [right ideal](../../../../../right-ideal.md) $B$. If $rB=0$, then $B\subseteq E$. Otherwise $rB$ is a nonzero [right ideal](../../../../../right-ideal.md), so it meets $cR$ nontrivially; lifting an element of that intersection gives a nonzero element of $B\cap E$. By the supplied assumption, $E$ contains some $d\in S$, giving

$$
rd=cb\qquad\text{for some }b\in R.
$$

This is the [right Ore condition](../../../../../right-ore-condition.md). The set $S$ is multiplicatively closed, and the denominator cancellation condition holds because its elements are [non-zero-divisors](../../../../../non-zero-divisor.md). Therefore [Ore theorem](../../../../../ore-theorem.md) constructs $Q$ and embeds $R$ in it.

For every [right ideal](../../../../../right-ideal.md) $J$ of $Q$,

$$
J=(J\cap R)Q.
$$

Indeed, if $x=as^{-1}\in J$, then $a=xs\in J\cap R$. Contracting an ascending chain of [right ideals](../../../../../right-ideal.md) of $Q$ to $R$ therefore proves that $Q$ is a [right Noetherian ring](../../../../../right-noetherian-ring.md).

Suppose $J$ is an [essential right ideal](../../../../../essential-right-ideal.md) of $Q$. For a nonzero [right ideal](../../../../../right-ideal.md) $B$ of $R$, choose $0\ne x\in J\cap BQ$. The [right Ore condition](../../../../../right-ore-condition.md) gives a common right denominator for a finite expression of $x$ in $BQ$, so there is $s\in S$ with

$$
0\ne xs\in B\cap(J\cap R).
$$

Thus $J\cap R$ is an [essential right ideal](../../../../../essential-right-ideal.md) of $R$. It contains a [regular element of a ring](../../../../../regular-element-of-a-ring.md), which becomes a [unit](../../../../../unit-in-a-ring.md) in $Q$, and consequently $J=Q$.

Finally, for any [right ideal](../../../../../right-ideal.md) $A$ of $Q$, choose by [Zorn lemma](../../../../../zorn-s-lemma.md) a [right ideal](../../../../../right-ideal.md) $B$ maximal subject to $A\cap B=0$. Then $A\oplus B$ is essential: a nonzero [right ideal](../../../../../right-ideal.md) disjoint from $A+B$ would enlarge $B$ while keeping it disjoint from $A$. Hence $A\oplus B=Q$. Every [submodule](../../../../../submodule.md) of the right regular [module](../../../../../module-mathematics.md) has a complement, making it a [semisimple module](../../../../../semisimple-module.md). Since it is also [Noetherian](../../../../../noetherian-ring.md), it is a finite [direct sum](../../../../../direct-sum.md) of [simple modules](../../../../../irreducible-module.md). It is therefore [Artinian](../../../../../artinian-ring.md), and $Q$ is a **semisimple Artinian ring**. This is [semisimplicity of a classical quotient from regular elements in essential ideals](../../../../../semisimplicity-of-a-classical-quotient-from-regular-elements-in-essential-ideals.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
