<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The polynomial is [Eisenstein](../../../../../../eisenstein-criterion.md) at $2$: every nonleading coefficient is even, and its constant term $126$ is not divisible by $4$. Therefore it is irreducible over $\mathbb Q$ and

$$
\boxed{[M:\mathbb Q]=5.}
$$

By part (a), the number of primes above a rational prime is the number of irreducible factors over the corresponding $p$-adic field.

We use the [Newton polygon](../../../../../../newton-polygon.md) theorem in this form: a segment of slope $-r$ and horizontal length $d$ accounts for $d$ roots of valuation $r$, counted with multiplicity, in an algebraic closure with $v_p(p)=1$. We also use the [denominator criterion for Newton polygon irreducibility](../../../../../../denominator-criterion-for-newton-polygon-irreducibility.md): if all roots have valuation $a/n$ with $\gcd(a,n)=1$, any monic factor of degree $d$ has constant-term valuation $da/n\in\mathbb Z$, hence $n\mid d$.

At $3$, the nonzero coefficient points are

$$
(0,2),\ (2,2),\ (3,1),\ (5,0).
$$

The lower hull is the single segment from $(0,2)$ to $(5,0)$, with slope $-2/5$. All five roots therefore have valuation $2/5$. A proper factor of degree $d$ would require $5\mid d$, which is impossible for $1\leq d<5$. Thus $g$ is irreducible over $\mathbb Q_3$, giving

$$
\boxed{\#\{\mathfrak q\subset\mathcal O_M:\mathfrak q\mid3\}=1.}
$$

The completion has ramification index $5$ and residue degree $1$: the value $2/5$ forces its ramification index to be divisible by $5$, and its degree is $5$.

At $7$, the nonzero coefficient points are

$$
(0,1),\ (2,1),\ (3,0),\ (5,0).
$$

The lower hull consists of a length-three segment of slope $-1/3$ and a length-two horizontal segment. Thus three roots have valuation $1/3$, and two have valuation zero. Reduction gives

$$
\bar g(T)=T^3(T^2-1)=T^3(T-1)(T+1)\quad\text{in }\mathbb F_7[T].
$$

Both $1$ and $-1$ are simple roots, so the [Hensel lemma](../../../../../../hensel-s-lemma.md) gives two distinct linear factors over $\mathbb Q_7$. The remaining cubic accounts for all the valuation-$1/3$ roots and is irreducible by the same denominator argument. Hence the local factor degrees are $1,1,3$, and

$$
\boxed{\#\{\mathfrak q\subset\mathcal O_M:\mathfrak q\mid7\}=3.}
$$

The two linear factors give $(e,f)=(1,1)$, and the cubic gives $(e,f)=(3,1)$. These data sum to degree five, as required. This computes the [local prime decomposition of T5 plus 6T3 plus 252T2 plus 126](../../../../../../local-prime-decomposition-of-t5-plus-6t3-plus-252t2-plus-126.md). Counting distinct factors merely modulo $3$ would not justify the result, since that reduction is $T^5$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
