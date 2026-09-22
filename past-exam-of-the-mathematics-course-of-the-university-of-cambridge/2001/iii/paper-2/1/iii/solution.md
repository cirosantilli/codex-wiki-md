<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [noncommutative domain](../../../../../../noncommutative-domain.md) $R$, the right [Ore condition](../../../../../../ore-condition.md) on its nonzero elements requires that for every $a\in R$ and nonzero $s$, there exist $t\ne0$ and $b\in R$ with $at=sb$. The [Ore theorem](../../../../../../ore-theorem.md) says that this is precisely the condition for a [division ring](../../../../../../division-ring.md) of right fractions in which $R$ embeds and every element is $as^{-1}$. The left-handed condition similarly gives left fractions.

For completeness, a [right Noetherian domain](../../../../../../right-noetherian-domain.md) satisfies the condition. If $aR\cap bR=0$ with $a,b\ne0$, the [right ideals](../../../../../../right-ideal.md)

$$
bR\subset bR+abR\subset bR+abR+a^2bR\subset\cdots
$$

form a strict chain of direct sums. Indeed, in a relation $\sum_{i=0}^na^ibr_i=0$, the first term lies in $bR$ and the rest in $aR$. Their zero intersection makes $br_0=0$, hence $r_0=0$; cancel $a$ and repeat. Every new summand is nonzero in a [noncommutative domain](../../../../../../noncommutative-domain.md), contradicting the [ascending chain condition](../../../../../../ascending-chain-condition.md). Thus $au=bv\ne0$ exists, with $u,v\ne0$, giving right common multiples. The opposite-ring argument gives left common multiples when $R$ is a [left Noetherian ring](../../../../../../left-noetherian-ring.md). This proves [right Noetherian domains satisfy the Ore condition](../../../../../../right-noetherian-domains-satisfy-the-ore-condition.md).

A sketch of the fraction construction also explains the theorem. Pairs $(a,s)$ represent $as^{-1}$. They represent the same fraction when a common right denominator $su=tv\ne0$ also satisfies $au=bv$. Addition uses $(au+bv)(su)^{-1}$. For multiplication choose $sc=bd$ with $d\ne0$; then

$$
(as^{-1})(bt^{-1})=ac(td)^{-1}.
$$

Further common denominators prove well-definedness and the [ring](../../../../../../ring.md) identities. The original map is injective because all nonzero denominators are regular; a zero fraction numerator would satisfy $au=0$ for $u\ne0$. Every nonzero fraction has inverse $sa^{-1}$, so the [ring](../../../../../../ring.md) is a [division ring](../../../../../../division-ring.md). This construction has the [universal property](../../../../../../universal-property.md) of inverting all nonzero elements.

Apply this to the two-sided [Noetherian](../../../../../../noetherian-ring.md) [noncommutative domain](../../../../../../noncommutative-domain.md) $kG$. Its left Ore property expresses any right fraction as a left one: choose $u\ne0$ with $ua=bs$, yielding $as^{-1}=u^{-1}b$. Hence **one [division ring](../../../../../../division-ring.md) is simultaneously the left and right classical [ring](../../../../../../ring.md) of quotients of $kG$**; the two constructions agree by their [universal property](../../../../../../universal-property.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
