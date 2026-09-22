<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $E:y^2=x^3-x^2+25x$, the addition formulas give

$$
P+T=(25,-125),
\qquad
Q+T=(5,-15)=-Q,
\qquad
P+Q=(5/4,-45/8).
$$

In particular, $[2]Q=T$ and $Q$ has order four, while the nonintegral coordinate of $[2]P=(144/25,-2172/125)$ and part (a) show that $P$ has infinite order.

For [two-isogeny descent](../../../../../../two-isogeny-descent.md), write

$$
E:y^2=x^3+ax^2+bx,
\qquad
E':y^2=x^3-2ax^2+(a^2-4b)x.
$$

The rational point $(0,0)$ is the kernel of a degree-two isogeny $E\to E'$. The square-class maps send an affine point with $x\ne0$ to $[x]\in\mathbb Q^*/\mathbb Q^{*2}$, send $O$ to $1$, and send $(0,0)$ to $[b]$ or $[a^2-4b]$ on the two curves. Their images determine the rank through

$$
2^r=\frac{|\alpha(E(\mathbb Q))|\,|\alpha'(E'(\mathbb Q))|}{4}.
$$

Here

$$
E':y^2=x^3+2x^2-99x.
$$

On $E$, the possible square classes divide $25$; real solubility excludes the negative classes, while $P$ and $Q$ exhibit $1$ and $5$. Thus $\alpha(E(\mathbb Q))=\{1,5\}$. On $E'$, the points

$$
(0,0),\quad(-1,10),\quad(11,22)
$$

exhibit the classes $-11,-1,11$, along with $1$. The remaining candidate classes are divisible by $3$. Their homogeneous spaces

$$
N^2=dU^4+2U^2V^2-\frac{99}{d}V^4
$$

have no primitive solution modulo $9$: reduction modulo $3$ first forces $3\mid UV$, and then the equation is congruent to $3$ or $6$ modulo $9$. Hence

$$
\alpha'(E'(\mathbb Q))=\{1,-1,11,-11\}.
$$

The rank formula gives $2^r=2\cdot4/4=2$, so $r=1$.

At the good primes $7$ and $19$, direct counts give

$$
\#E(\mathbb F_7)=12,
\qquad
\#E(\mathbb F_{19})=16.
$$

The [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) injects rational torsion into both groups, so its order divides $\gcd(12,16)=4$. Since $Q$ has order four, the torsion subgroup is $\mathbb Z/4\mathbb Z$. Therefore

$$
E(\mathbb Q)\cong\mathbb Z/4\mathbb Z\times\mathbb Z,
$$

so $t=1$, $d_1=4$, and $r=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
