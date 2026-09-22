<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A right [Ore localization](../../../../../ore-localization.md) at $S$ is a unital homomorphism $\iota:R\to Q$ such that every $\iota(s)$, $s\in S$, is a [unit](../../../../../unit-in-a-ring.md), every element of $Q$ is $\iota(r)\iota(s)^{-1}$, and

$$
\ker\iota=\{r\in R:rt=0\text{ for some }t\in S\}.
$$

Equivalently, the usual fraction construction has this zero criterion and is universal among homomorphisms that invert $S$. Injectivity is required only when the denominators are [regular elements of a ring](../../../../../regular-element-of-a-ring.md). If $0\in S$, every homomorphism inverting $S$ has zero target; this is the degenerate zero-ring localization. For a nonzero localization we require $0\notin S$.

The necessary and sufficient conditions are that $S$ be a [right denominator set](../../../../../right-denominator-set.md):

- For $r\in R$ and $s\in S$, there are $t\in S$ and $b\in R$ with $rt=sb$; this is the [right Ore condition](../../../../../right-ore-condition.md).
- If $sr=0$ with $s\in S$, there is $t\in S$ with $rt=0$; this is right reversibility.

For necessity, write the element $\iota(s)^{-1}\iota(r)$ as $\iota(b)\iota(t)^{-1}$. Multiplying by $\iota(s)$ on the left and $\iota(t)$ on the right gives $\iota(rt-sb)=0$. The zero criterion supplies $u\in S$ with $(rt-sb)u=0$. Hence $r(tu)=s(bu)$, the [right Ore condition](../../../../../right-ore-condition.md) in $R$, not merely an equality of images in $Q$. Also $sr=0$ makes $\iota(r)=0$ because $\iota(s)$ is invertible, and the zero criterion gives $rt=0$. This proves both necessities.

The sufficiency is the [Ore theorem](../../../../../ore-theorem.md) for denominator sets. Concretely, right fractions can be represented by $(r,s)$; a common-denominator equality has $su=tv\in S$ and $ru=r'v$ for suitable $u,v\in R$. The two conditions make the induced fraction equivalence transitive and make addition and multiplication well defined; the zero fraction is exactly the kernel displayed above. The requested direction of the theorem was necessity, for which the complete argument has just been given.

For a [right Noetherian domain](../../../../../right-noetherian-domain.md), any two nonzero principal [right ideals](../../../../../right-ideal.md) intersect. To see this without using the desired localization, suppose $bR\cap aR=0$ with $a,b\ne0$. The sum

$$
bR+abR+a^2bR+\cdots
$$

is direct: reduce a finite relation modulo $aR$ to get its first summand zero, then cancel $a$ in the [noncommutative domain](../../../../../noncommutative-domain.md) and repeat. Every summand is nonzero, so the finite partial sums form a strictly ascending chain of [right ideals](../../../../../right-ideal.md), contradicting the [ascending chain condition](../../../../../ascending-chain-condition.md). A nonzero intersection $rR\cap sR$ thus provides $rt=sb\ne0$, with $t\ne0$. This is the [right Ore condition](../../../../../right-ore-condition.md) for $S=R\setminus\{0\}$. Reversibility is automatic in a [noncommutative domain](../../../../../noncommutative-domain.md), and the zero criterion makes the map injective. The localization is a [division ring](../../../../../division-ring.md), since a nonzero $rs^{-1}$ has inverse $sr^{-1}$.

The [Goldie theorem](../../../../../goldie-s-theorem.md) states that a [semiprime ring](../../../../../semiprime-ring.md) has a semisimple Artinian [classical right ring of quotients](../../../../../classical-right-ring-of-quotients.md) if and only if it has finite right [uniform dimension](../../../../../uniform-dimension.md) and satisfies the [ascending chain condition](../../../../../ascending-chain-condition.md) on [right annihilators](../../../../../right-annihilator.md). A [right Noetherian ring](../../../../../right-noetherian-ring.md) satisfies the annihilator condition because [right annihilators](../../../../../right-annihilator.md) are [right ideals](../../../../../right-ideal.md). Its right regular [module](../../../../../module-mathematics.md) has finite [uniform dimension](../../../../../uniform-dimension.md): an infinite direct sum of nonzero submodules would give a strictly ascending chain of finite partial sums. A [prime ring](../../../../../prime-ring.md) is [semiprime](../../../../../semiprime.md), so the theorem applies to a prime [right Noetherian ring](../../../../../right-noetherian-ring.md) $R$.

To obtain a single matrix-ring factor, not just a finite product, prove that its quotient $Q$ is prime. A nonzero two-sided [ideal](../../../../../ideal.md) $I\subseteq Q$ contains a nonzero fraction $rs^{-1}$ and hence the nonzero element $r=(rs^{-1})s\in I\cap R$. The same holds for any other nonzero [ideal](../../../../../ideal.md) $K$. Since $R$ is prime, $(I\cap R)(K\cap R)\ne0$, so $IK\ne0$. Thus $Q$ is prime. The [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) gives a finite product of matrix rings over [division rings](../../../../../division-ring.md); primeness excludes two different nonzero factors with zero product. This proves the [prime classical quotient of a prime right Goldie ring](../../../../../prime-classical-quotient-of-a-prime-right-goldie-ring.md):

$$
\boxed{Q_{\mathrm{cl}}^r(R)\cong M_n(D)\quad\text{for a division ring }D.}
$$

For the requested counterexample to Noetherianity, take $R=k[x_1,x_2,\ldots]$. It is a commutative [integral domain](../../../../../integral-domain.md) and has its [field of fractions](../../../../../field-of-fractions.md) as its [classical right ring of quotients](../../../../../classical-right-ring-of-quotients.md). But $(x_1)\subsetneq(x_1,x_2)\subsetneq\cdots$ is a strictly ascending ideal chain: evaluation at $x_1=\cdots=x_m=0$ shows $x_{m+1}$ is not in the preceding [ideal](../../../../../ideal.md). Therefore existence of a classical quotient does **not** imply right Noetherianity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 85](../../paper-85-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
