<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The denominator is $\pi^nX$; dividing by $X$ removes the zero at $X=0$. A [uniformizer](../../../../../../uniformizer.md) of a degree-$n$ totally ramified extension generates the field: its [valuation](../../../../../../valuation.md) over $K$ is $1/n$, so $K(\pi)/K$ already has ramification index at least $n$. Hence $K(\pi)=L$, its [minimal polynomial](../../../../../../minimal-polynomial.md) has degree $n$, and its conjugates are the distinct $\sigma(\pi)$ for $\sigma\in G$.

Factor the [minimal polynomial](../../../../../../minimal-polynomial.md) over $L$. The [reduced ramification polynomial](../../../../../../reduced-ramification-polynomial.md) is

$$
g(X)=\frac{f(\pi(1+X))}{\pi^nX}=\prod_{\sigma\ne1}\left(X-\frac{\sigma(\pi)-\pi}{\pi}\right).
$$

Every displayed root $r_\sigma=(\sigma(\pi)-\pi)/\pi$ is nonzero and integral, since two [uniformizers](../../../../../../uniformizer.md) have a difference of [valuation](../../../../../../valuation.md) at least one. Thus $g$ is monic of degree $n-1$, has nonzero constant coefficient, and belongs to $\mathcal O_L[X]$. For $n=1$ it is the constant [polynomial](../../../../../../polynomial-split.md) $1$, with no slopes and no ramification jumps.

Here is also a justification of the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) in this setting. The powers $1,\pi,\ldots,\pi^{n-1}$ are a $K$-basis. In an expansion $x=\sum a_j\pi^j$, the nonzero terms have [valuations](../../../../../../valuation.md) $nv_K(a_j)+j$, distinct modulo $n$; therefore there is no cancellation at the least [valuation](../../../../../../valuation.md). If $x$ is integral, all those values are nonnegative, which forces $a_j\in\mathcal O_K$. Thus $\mathcal O_L=\mathcal O_K[\pi]$. For $j\geq1$, $\sigma(\pi)^j-\pi^j$ is divisible by $\sigma(\pi)-\pi$, with the remaining factor integral. Consequently every $\sigma(x)-x$ has [valuation](../../../../../../valuation.md) at least $v_L(\sigma(\pi)-\pi)$, and equality is attained at $x=\pi$.

For a nonidentity automorphism, write $i(\sigma)=v_L(\sigma(\pi)-\pi)$. By the defining inequality for the [lower ramification numbering](../../../../../../lower-ramification-numbering.md),

$$
\sigma\in G_m\setminus G_{m+1}\quad\Longleftrightarrow\quad i(\sigma)=m+1\quad\Longleftrightarrow\quad v_L(r_\sigma)=m.
$$

The [Newton polygon root valuation theorem](../../../../../../newton-polygon-root-valuation-theorem.md) therefore proves the [ramification breaks from a reduced ramification polygon](../../../../../../ramification-breaks-from-a-reduced-ramification-polygon.md) relation:

$$
\boxed{-m\text{ is a slope of the coefficient-exponent }N_L(g)\quad\Longleftrightarrow\quad G_m\ne G_{m+1}.}
$$

The segment's horizontal length is exactly $|G_m|-|G_{m+1}|$. Equivalently, in the [reflected Newton polygon convention](../../../../../../reflected-newton-polygon-convention.md) required for a positive-slope formulation,

$$
\boxed{m\text{ is a slope of the reflected }N_L(g)\quad\Longleftrightarrow\quad G_m\ne G_{m+1}.}
$$

All occurring root [valuations](../../../../../../valuation.md) are nonnegative integers. For negative indices, extend $G_m=G$; total ramification means that there are no negative-index jumps, so the reflected formulation remains true for all integers.

The sign distinction is substantive. Using the [uniformizer](../../../../../../uniformizer.md) from question 2, whose [minimal polynomial](../../../../../../minimal-polynomial.md) is $X^6+3$, gives

$$
g(X)=\frac{(1+X)^6-1}{X}=6+15X+20X^2+15X^3+6X^4+X^5.
$$

Its coefficient [valuations](../../../../../../valuation.md) are $(6,6,0,6,6,0)$, because $v_L(3)=6$. The usual lower hull has vertices $(0,6),(2,0),(5,0)$ and slopes $-3,0$, of lengths $2,3$. These correspond exactly to the drops $|G_3|-|G_4|=2$ and $|G_0|-|G_1|=3$. With the reflected axis the slopes are $0,3$, as in the printed positive-$m$ wording. If the coefficient-exponent definition is used throughout, the printed assertion needs the minus sign shown above.

<a id="3/b/image-coefficient-exponent-and-reflected-newton-polygons-of-the-reduced-ramification-polynomial"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-123-newton-conventions.png)

**[Figure 1](#3/b/image-coefficient-exponent-and-reflected-newton-polygons-of-the-reduced-ramification-polynomial). Coefficient-exponent and reflected Newton polygons of the reduced ramification polynomial**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
