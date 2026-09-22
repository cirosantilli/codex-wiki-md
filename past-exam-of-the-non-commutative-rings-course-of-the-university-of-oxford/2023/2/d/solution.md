<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $D=\hat R$. We first check that this [noncommutative formal power series ring](../../../../noncommutative-formal-power-series-ring.md) is a [noncommutative domain](../../../../noncommutative-domain.md). For nonzero $F,G\in D$, let $p,q$ be the smallest lengths of [words](../../../../string.md) with nonzero coefficients in $F,G$, respectively. Their degree-$p$ and degree-$q$ parts $F_p,G_q$ are nonzero [homogeneous polynomials](../../../../homogeneous-polynomial.md) in the [free associative algebra](../../../../free-associative-algebra.md).

Choose [words](../../../../string.md) $u,v$ with nonzero coefficients in $F_p,G_q$. In $F_pG_q$, the coefficient of $uv$ is the product of those two coefficients: a [word](../../../../string.md) of length $p+q$ has a unique splitting into a prefix of length $p$ and a suffix of length $q$. This product is nonzero in $\mathbb Q$. The degree-$p+q$ part of $FG$ is exactly $F_pG_q$, since all lower parts of $F$ and $G$ vanish. Thus $FG\ne0$, proving that $D$ is a [noncommutative domain](../../../../noncommutative-domain.md).

By the defining property of the [free associative algebra](../../../../free-associative-algebra.md), there is a [ring homomorphism](../../../../ring-homomorphism.md)

$$
f:R\longrightarrow D,\qquad f(x_1)=1+x_1,\qquad f(x_2)=2+x_2.
$$

The same substitution defines a [ring automorphism](../../../../ring-automorphism.md) of $R$, with inverse $x_1\mapsto x_1-1$, $x_2\mapsto x_2-2$. Composing this [ring automorphism](../../../../ring-automorphism.md) with the natural inclusion $R\hookrightarrow D$ proves that $f$ is [injective](../../../../injective-function.md).

Finally,

$$
\begin{aligned}
f(x_1+x_2)&=3+x_1+x_2,& f(x_1-x_2)&=-1+x_1-x_2,\\
f(x_1)&=1+x_1,&f(x_2)&=2+x_2.
\end{aligned}
$$

Their [constant terms](../../../../constant-term.md) are $3,-1,1,2$, respectively, all nonzero. By the [unit criterion for noncommutative formal power series](../../../../unit-criterion-for-noncommutative-formal-power-series.md) proved in [c](../c.md), all four elements are [units](../../../../unit-in-a-ring.md). Therefore $D$ and $f$ have every required property. The embedding changes the images of the generators, so the failure of the original monomial [left Ore set](../../../../left-ore-set.md) in [b](../b.md) presents no obstruction.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the non-commutative rings course of the University of Oxford](../../../split.md)
5. [Non-commutative rings course of the University of Oxford](../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
