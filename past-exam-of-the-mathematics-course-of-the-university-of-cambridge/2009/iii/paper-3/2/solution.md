<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $S$ be a [multiplicative subset](../../../../../multiplicatively-closed-set.md), containing one and closed under products. On $A\times S$, use

$$
(a,s)\sim(b,t)\quad\Longleftrightarrow\quad u(ta-sb)=0\text{ for some }u\in S.
$$

The relation is reflexive and symmetric. For transitivity, if $u(ta-sb)=0$ and $v(rb-tc)=0$, then multiplication and addition give $uvt(ra-sc)=0$. Thus it is an [equivalence relation](../../../../../equivalence-relation.md). Write $a/s$ for the equivalence class. The [localization of a ring](../../../../../localization-of-a-ring.md) $A_S=S^{-1}A$ has operations

$$
\frac as+\frac bt=\frac{at+bs}{st},\qquad \frac as\frac bt=\frac{ab}{st},\qquad -\frac as=\frac{-a}{s}.
$$

They are well defined. For example, replacing $a/s$ by $b/t$ in its sum with $c/r$ gives cross-numerator difference $r^2(ta-sb)$, and in its product with $c/r$ gives $rc(ta-sb)$. The same annihilating element $u$ kills both differences. Replacing the other input works identically. Associativity and distributivity then follow by putting all terms over the product of their denominators and using the [ring](../../../../../ring.md) identities in $A$. Addition and multiplication are commutative, with identities $0/1$ and $1/1$, and the displayed negative is an additive inverse. Hence **$S^{-1}A$ is a commutative ring**. If $0\in S$, the fraction relation identifies all elements, producing the zero [ring](../../../../../ring.md).

The canonical [ring homomorphism](../../../../../ring-homomorphism.md) $\iota:A\to S^{-1}A$, $a\mapsto a/1$, makes each $s\in S$ a [unit](../../../../../unit-in-a-ring.md), with inverse $1/s$. The [universal property of localization](../../../../../universal-property-of-localization.md) states that any [ring homomorphism](../../../../../ring-homomorphism.md) $h:A\to C$ sending $S$ into the [units](../../../../../unit-in-a-ring.md) factors uniquely through $\iota$. Define the factor by

$$
\boxed{\widetilde h(a/s)=h(a)h(s)^{-1}.}
$$

If $u(ta-sb)=0$, then $h(u)$ is invertible, so $h(t)h(a)=h(s)h(b)$, proving well-definedness. The fraction operations prove that $\widetilde h$ is a [ring homomorphism](../../../../../ring-homomorphism.md). Its value is forced by $a/s=\iota(a)\iota(s)^{-1}$, so it is unique. This property characterizes the [localization](../../../../../localization-of-a-ring.md) up to a unique compatible [isomorphism](../../../../../isomorphism.md).

For a [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$, its complement is a [multiplicative subset](../../../../../multiplicatively-closed-set.md), and the [localization at a prime ideal](../../../../../localization-at-a-prime-ideal.md) is **$A_{\mathfrak p}=(A\setminus\mathfrak p)^{-1}A$**. Fractions with numerator outside $\mathfrak p$ are [units](../../../../../unit-in-a-ring.md); those with numerator in $\mathfrak p$ form the unique [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak pA_{\mathfrak p}$. Thus it is a [local ring](../../../../../local-ring.md).

For the nilpotent question, suppose $a\ne0$ and $a^n=0$. Its [annihilator](../../../../../annihilator-ring-theory.md) is a proper [ideal](../../../../../ideal.md), so it lies in some [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak m$. The fraction criterion says $a/1=0$ in $A_{\mathfrak m}$ only if $sa=0$ for some $s\notin\mathfrak m$, which is impossible by the choice of $\mathfrak m$. Thus $a/1$ is a nonzero [nilpotent element](../../../../../nilpotent.md) in that [localization](../../../../../localization-of-a-ring.md). This proves [reducedness is detected by prime localizations](../../../../../reducedness-is-detected-by-prime-localizations.md): **if every prime localization is reduced, $A$ has no nonzero nilpotent elements**.

For the domain question take $A=k\times k$ with $k$ a [field](../../../../../field.md). Its only [prime ideals](../../../../../prime-ideal.md) are $\mathfrak p_1=0\times k$ and $\mathfrak p_2=k\times0$: a [prime ideal](../../../../../prime-ideal.md) must contain one of the orthogonal [idempotents](../../../../../idempotent.md) $(1,0),(0,1)$, and the corresponding quotient is $k$. Localizing at $\mathfrak p_1$ makes $(1,0)$ invertible and kills $(0,1)$, giving $A_{\mathfrak p_1}\cong k$; similarly $A_{\mathfrak p_2}\cong k$. But $(1,0)(0,1)=0$ with both factors nonzero. Therefore **domain prime localizations do not force $A$ to be an integral domain**, as expressed by [domain prime localizations do not imply a domain](../../../../../domain-prime-localizations-do-not-imply-a-domain.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
