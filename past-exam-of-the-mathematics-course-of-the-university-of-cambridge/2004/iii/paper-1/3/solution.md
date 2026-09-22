<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use generators $x,D$ with $Dx-xD=1$. The ordered [monomials](../../../../../monomial.md) $x^iD^j$ form a [basis](../../../../../basis.md): construct the [Weyl algebra](../../../../../weyl-algebra.md) as the differential [Ore extension](../../../../../ore-extension.md) of $\mathbb C[x]$ with $Df=fD+f'$, which has unique ordered polynomial expressions. Giving both generators degree one produces the [Bernstein filtration](../../../../../bernstein-filtration.md), whose [associated graded ring](../../../../../associated-graded-ring.md) is $\mathbb C[x,\xi]$. If $a,b\ne0$, their nonzero leading symbols have nonzero product in this polynomial [integral domain](../../../../../integral-domain.md). Thus $ab$ has nonzero leading symbol and cannot vanish. Hence **$A_1(\mathbb C)$ has no nontrivial [zero divisors](../../../../../zero-divisor.md)**.

Here is the left-handed [Ore theorem](../../../../../ore-theorem.md). Let $S$ be a multiplicative set of [regular elements of a ring](../../../../../regular-element-of-a-ring.md), containing $1$ and excluding $0$. There is an injective [Ore localization](../../../../../ore-localization.md) whose elements are left fractions $s^{-1}a$ if and only if

$$
\boxed{\text{for every }a\in A,s\in S,\text{ there are }t\in S,b\in A\text{ with }ta=bs.}
$$

This is the left [Ore condition](../../../../../ore-condition.md). For a [noncommutative domain](../../../../../noncommutative-domain.md), taking $S=A\setminus\{0\}$ gives a [division ring](../../../../../division-ring.md) exactly when this condition holds. With zero-divisor denominators a further left reversibility condition is needed; the regular-denominator statement is the one used here.

Necessity follows by writing $as^{-1}=t^{-1}b$ in the quotient and multiplying by $t$ and $s$, giving $ta=bs$ in the embedded original [ring](../../../../../ring.md). For a construction proving sufficiency, use the [left Ore fraction construction](../../../../../left-ore-fraction-construction.md): pairs $(s,a)$ represent $s^{-1}a$, and $(s,a)$ and $(t,b)$ are equivalent when

$$
us=vt=w\in S,\qquad ua=vb
$$

for suitable $u,v\in A$. Reflexivity and symmetry are immediate. For transitivity, combine $us=vt=w$ and $u't=v'q=w'$ by a common left multiple $hw=kw'\in S$. Then $(hv-ku')t=0$, so regularity gives $hv=ku'$, which combines the numerator equalities and proves transitivity.

Addition uses the common denominator $w$, with numerator $ua+vb$. To multiply $s^{-1}a$ by $t^{-1}b$, choose $v\in S,c\in A$ with $va=ct$; set

$$
(s^{-1}a)(t^{-1}b)=(vs)^{-1}cb.
$$

The [Ore condition](../../../../../ore-condition.md) supplies a common refinement whenever a representative or an Ore relation is changed, and regularity cancels the shared denominator, proving independence of choices. The same refinements verify the [ring](../../../../../ring.md) axioms; the formulas are simply addition and multiplication after clearing left denominators. The map $a\mapsto(1,a)$ is injective, since equivalence to zero would give $ua=0$ with $u\in S$. Each $s\in S$ becomes invertible. A homomorphism inverting $S$ extends uniquely by $(s,a)\mapsto f(s)^{-1}f(a)$, giving the universal property. For all nonzero denominators in a [noncommutative domain](../../../../../noncommutative-domain.md), a nonzero fraction has inverse $(s^{-1}a)^{-1}=a^{-1}s$, so the quotient is a [division ring](../../../../../division-ring.md). This is the requested proof sketch, with the fraction equivalence and multiplication made explicit.

It remains to check the left [Ore condition](../../../../../ore-condition.md) for $A_1(\mathbb C)$. Its graded polynomial [ring](../../../../../ring.md) is [Noetherian](../../../../../noetherian-ring.md) by the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md). Lifting homogeneous generators of a graded [left ideal](../../../../../left-ideal.md) and successively cancelling leading symbols proves that the filtered [algebra](../../../../../algebra-split.md) is a [left Noetherian ring](../../../../../left-noetherian-ring.md): each subtraction lowers the nonnegative degree, so it terminates.

In any left Noetherian [noncommutative domain](../../../../../noncommutative-domain.md), nonzero principal [left ideals](../../../../../left-ideal.md) intersect. Otherwise $Ab\cap Aa=0$ with $a,b\ne0$ would make

$$
Ab\oplus Aba\oplus Aba^2\oplus\cdots
$$

an infinite direct sum of nonzero [left ideals](../../../../../left-ideal.md). To verify directness, reduce a finite relation modulo $Aa$ to make its first summand zero, then cancel $a$ on the right and repeat. Its increasing finite partial sums contradict the [ascending chain condition](../../../../../ascending-chain-condition.md). A nonzero element of $Aa\cap As$ therefore has the form $ta=bs\ne0$, with $t\ne0$, proving the required condition. Consequently **$A_1(\mathbb C)$ has a classical [ring](../../../../../ring.md) of left quotients, and it is a division [ring](../../../../../ring.md)**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
