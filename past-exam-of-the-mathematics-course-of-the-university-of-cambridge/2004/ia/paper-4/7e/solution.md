<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The [binomial polynomial](../../../../../binomial-polynomial.md) $P_r$ equals $1$ when $r=0$. For $n\geq0$, it has value $\binom nr$ if $r\leq n$ and value zero otherwise. These are [integers](../../../../../integer.md). If $n=-k<0$, then

$$
P_r(-k)=(-1)^r\frac{k(k+1)\cdots(k+r-1)}{r!}
=(-1)^r\binom{k+r-1}{r}\in\mathbb Z.
$$

Hence each $P_r$ is an [integer-valued polynomial](../../../../../integer-valued-polynomial.md) on all of $\mathbb Z$, including negative arguments.

For $r\geq1$, factor the common product in the two [polynomials](../../../../../polynomial-split.md):

$$
P_r(X)-P_r(X-1)
=\frac{(X-1)\cdots(X-r+1)}{r!}\bigl[X-(X-r)\bigr]
=P_{r-1}(X-1).
$$

For $r=1$ the common product is empty and equals $1$, so this argument also covers that boundary case.

The [polynomial](../../../../../polynomial-split.md) $P_r$ has [polynomial degree](../../../../../degree-of-a-polynomial.md) $r$ and [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $1/r!$. For a [polynomial](../../../../../polynomial-split.md) $F$ of [polynomial degree](../../../../../degree-of-a-polynomial.md) $d$ with [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $a_d\in\mathbb Q$, subtract $d!a_dP_d$; the remainder has smaller [polynomial degree](../../../../../degree-of-a-polynomial.md). Repeating gives the required expansion with [rational numbers](../../../../../rational-number.md) $c_r$. For uniqueness, suppose two expansions differ and let $s$ be the largest index with different coefficients. Their difference then has a nonzero term of [polynomial degree](../../../../../degree-of-a-polynomial.md) $s$, with [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) equal to that coefficient difference divided by $s!$. It cannot be the zero [polynomial](../../../../../polynomial-split.md). Thus the expansion is unique.

Replacing $X$ by $X+1$ in the earlier identity gives $\Delta P_r(X)=P_{r-1}(X)$ for $r\geq1$, while $\Delta P_0=0$. By linearity of the [forward difference operator](../../../../../forward-difference-operator.md),

$$
\boxed{\Delta F(X)=\sum_{r=0}^{d-1}c_{r+1}(F)P_r(X).}
$$

An empty sum is zero when $d=0$. If $H=F-G$ were nonconstant, with [polynomial degree](../../../../../degree-of-a-polynomial.md) $s\geq1$ and [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $a_s$, then $\Delta H$ would have [polynomial degree](../../../../../degree-of-a-polynomial.md) $s-1$ and [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $sa_s\ne0$. Therefore $\Delta F=\Delta G$ [forces](../../../../../force.md) $H$ to be constant.

There is a direct way to recover every coefficient. Since $P_0(0)=1$ and $P_j(0)=0$ for $j\geq1$, repeated application of the [forward difference operator](../../../../../forward-difference-operator.md) gives

$$
\boxed{c_r(F)=\Delta^r F(0)=\sum_{j=0}^r(-1)^{r-j}\binom rj F(j).}
$$

The last equality follows by expanding $(T-I)^r$, where $TF(X)=F(X+1)$; the commuting shifts obey the [binomial theorem](../../../../../binomial-theorem.md). If $F$ is an [integer-valued polynomial](../../../../../integer-valued-polynomial.md), every summand on the right is an [integer](../../../../../integer.md), proving that all $c_r(F)$ are [integers](../../../../../integer.md). Together with the first paragraph this gives both directions of the [Newton series for an integer-valued polynomial sequence](../../../../../newton-series-for-an-integer-valued-polynomial-sequence.md) description.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
