# Remainder of polynomial division

↑ **Parent:** [Polynomial division](polynomial-division.md)

The polynomial remainder is the [polynomial](polynomial-split.md) $r$ in [polynomial division](polynomial-division.md) $q=Qs+r$. Division by $X-a$ has a constant [polynomial remainder](remainder-of-polynomial-division.md) $q(a)$, as expressed by the [factor theorem](factor-theorem.md).

For any identity $f=gq+r$, [polynomial evaluation](polynomial-evaluation.md) at a [root of a polynomial](root-of-a-polynomial.md) $a$ of $g$ gives

$$
f(a)=g(a)q(a)+r(a)=r(a).
$$

This substitution requires no division by $g(a)$. In the worked example, [polynomial factorization](factorization-of-polynomials.md) gives $g=(X-1)(X+2)$, so its two [roots of a polynomial](root-of-a-polynomial.md) are $1$ and $-2$. The cubic [polynomial](polynomial-split.md) and its linear [polynomial remainder](remainder-of-polynomial-division.md) agree there:

$$
\begin{aligned}
f(1)&=2+3-5+6=6=r(1),\\
f(-2)&=-16+12+10+6=12=r(-2).
\end{aligned}
$$

A cubic expression has been compressed into a straight line carrying exactly these two values.

<a id="image-the-original-polynomial-f-and-its-polynomial-remainder-r-agree-at-both-polynomial-roots-of-g-because-f-r-gq-vanishes-there"></a>
![](polynomial-remainder-evaluation.png)

**[Figure 12](#image-the-original-polynomial-f-and-its-polynomial-remainder-r-agree-at-both-polynomial-roots-of-g-because-f-r-gq-vanishes-there). The original polynomial $f$ and its polynomial remainder $r$ agree at both polynomial roots of $g$ because $f-r=gq$ vanishes there**.

Conversely, those two values determine the linear [polynomial remainder](remainder-of-polynomial-division.md) by [polynomial interpolation](polynomial-interpolation.md). Write $r=AX+B$; then $A+B=6$ and $-2A+B=12$, giving $A=-2$ and $B=8$. The [polynomial degree](degree-of-a-polynomial.md) bound is essential: adding any multiple of $g$ preserves the two values, but generally raises the [polynomial degree](degree-of-a-polynomial.md). The plot also shows agreement at $x=-1/2$, where $q=0$ rather than $g=0$. Agreement of $f$ and $r$ at a point therefore does not imply that the point is a [root of a polynomial](root-of-a-polynomial.md) of the divisor.

**Table of contents**

- [Polynomial remainder theorem](polynomial-remainder-theorem.md)

## ↑ Ancestors (6)

1. [Polynomial division](polynomial-division.md)
2. [Polynomial](polynomial-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
