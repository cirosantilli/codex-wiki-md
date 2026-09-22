<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [commutative ring](../../../../../commutative-ring.md) $R$ and a [multiplicative subset](../../../../../multiplicatively-closed-set.md) $S$ containing $1$, the [universal property of localization](../../../../../universal-property-of-localization.md) specifies a pair $(R_S,\iota)$ with $\iota:R\to R_S$ a unital [ring homomorphism](../../../../../ring-homomorphism.md), such that every $\iota(s)$, $s\in S$, is a [unit](../../../../../unit-in-a-ring.md), and any unital [ring homomorphism](../../../../../ring-homomorphism.md) $f:R\to T$ into a commutative [ring](../../../../../ring.md) that sends $S$ to [units](../../../../../unit-in-a-ring.md) factors uniquely through $\iota$. Thus there is a unique $\widetilde f:R_S\to T$ satisfying $\widetilde f\iota=f$. The property determines the pair up to a unique compatible [isomorphism](../../../../../isomorphism.md).

For existence, take pairs $(r,s)\in R\times S$ and declare

$$
(r,s)\sim(r',s')\quad\Longleftrightarrow\quad u(s'r-sr')=0\text{ for some }u\in S.
$$

The extra multiplier is essential when $R$ has [zero divisors](../../../../../zero-divisor.md). This is an [equivalence relation](../../../../../equivalence-relation.md): for transitivity, multiply the two cross-multiplication equations by appropriate denominators and add them, using the product of their annihilating multipliers. Write the class as $r/s$ and define

$$
\frac rs+\frac{r'}{s'}=\frac{rs'+r's}{ss'},\qquad\frac rs\frac{r'}{s'}=\frac{rr'}{ss'},\qquad\iota(r)=\frac r1.
$$

Multiplying the defining equivalence equations verifies that these operations are well defined. They give a [commutative ring](../../../../../commutative-ring.md), and $s/1$ has inverse $1/s$. The required map is necessarily

$$
\widetilde f(r/s)=f(r)f(s)^{-1}.
$$

It is well defined because applying $f$ to $u(s'r-sr')=0$ and cancelling the units $f(u),f(s),f(s')$ equates the two images. Its addition and multiplication laws follow directly from the fraction formulas. This establishes existence and the [universal property of localization](../../../../../universal-property-of-localization.md). If $0\in S$, this construction gives the zero [ring](../../../../../ring.md), which is allowed as a localization.

For a [prime ideal](../../../../../prime-ideal.md) $P$, its complement $S=R\setminus P$ is multiplicatively closed, and [localization at a prime ideal](../../../../../localization-at-a-prime-ideal.md) means $R_P=S^{-1}R$. The map

$$
R_P\longrightarrow\operatorname{Frac}(R/P),\qquad r/s\longmapsto\overline r/\overline s
$$

is well defined and surjective, with [kernel of a ring homomorphism](../../../../../kernel-of-a-ring-homomorphism.md) $PR_P$: a numerator has zero image exactly when it belongs to $P$. Since $R/P$ is an [integral domain](../../../../../integral-domain.md), its [field of fractions](../../../../../field-of-fractions.md) is a nonzero [field](../../../../../field.md), so $PR_P$ is a proper [maximal ideal](../../../../../maximal-ideal.md). Every fraction $r/s$ with $r\notin P$ is a [unit](../../../../../unit-in-a-ring.md), with inverse $s/r$. Every fraction with $r\in P$ belongs to this proper ideal and cannot be a [unit](../../../../../unit-in-a-ring.md). Thus the nonunits are exactly $PR_P$, and every proper ideal lies within it. Consequently

$$
\boxed{R_P\text{ is a local ring with unique maximal ideal }PR_P.}
$$

Now suppose each $R_P$ is [reduced](../../../../../reduced-ring.md). If $x\in R$ is [nilpotent](../../../../../nilpotent.md), its image $x/1$ is [nilpotent](../../../../../nilpotent.md) in every $R_P$, hence is zero. If $x\ne0$, its [annihilator](../../../../../annihilator-ring-theory.md) $\operatorname{Ann}_R(x)$ is a proper ideal, so choose a [maximal ideal](../../../../../maximal-ideal.md) $P$ containing it. Maximal ideals in a [commutative ring](../../../../../commutative-ring.md) are [prime ideals](../../../../../prime-ideal.md). The [vanishing criterion in a module localization](../../../../../vanishing-criterion-in-a-module-localization.md) would give $sx=0$ for some $s\notin P$. But then $s\in\operatorname{Ann}_R(x)\subseteq P$, a contradiction. Hence **$R$ is reduced**. This is [reducedness is detected by prime localizations](../../../../../reducedness-is-detected-by-prime-localizations.md); no finiteness hypothesis is needed.

The stronger local-domain condition does not force $R$ to be an [integral domain](../../../../../integral-domain.md). Take $R=k\times k$ for a [field](../../../../../field.md) $k$. Its only [prime ideals](../../../../../prime-ideal.md) are $P_1=0\times k$ and $P_2=k\times0$: a [prime ideal](../../../../../prime-ideal.md) must contain one of the orthogonal [idempotents](../../../../../idempotent.md) $(1,0)$ and $(0,1)$, and the remaining quotient is the [field](../../../../../field.md) $k$. At $P_1$, inverting $(1,0)$ kills the second component, so $R_{P_1}\cong k$; similarly $R_{P_2}\cong k$. Both localizations are [integral domains](../../../../../integral-domain.md), but

$$
(1,0)(0,1)=0
$$

is a product of nonzero elements in $R$. Therefore **the answer is no**, as illustrated by [domain prime localizations do not imply a domain](../../../../../domain-prime-localizations-do-not-imply-a-domain.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
