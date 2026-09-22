<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use [two-isogeny descent](../../../../../two-isogeny-descent.md), stating the arithmetic results involved. For

$$
E:y^2=x(x^2+ax+b),\qquad
E':Y^2=X(X^2-2aX+a^2-4b),
$$

define the [two-torsion square-class homomorphism](../../../../../two-torsion-square-class-homomorphism.md) $\alpha_E:E(\mathbb Q)\to\mathbb Q^\times/\mathbb Q^{\times2}$ by $\alpha_E(o)=1$, $\alpha_E((0,0))=b$, and $\alpha_E((x,y))=x$ otherwise. Its kernel is the image of the dual [two-isogeny formula](../../../../../two-isogeny-formula.md); the analogous map $\alpha_{E'}$ has kernel the image of the forward [two-isogeny formula](../../../../../two-isogeny-formula.md). The [two-isogeny rank formula](../../../../../square-class-index-formula-for-two-isogeny-descent.md) is

$$
2^r=\frac{|\alpha_E(E(\mathbb Q))|\,
|\alpha_{E'}(E'(\mathbb Q))|}{4}.
$$

The images have signed squarefree representatives supported on [primes](../../../../../prime-number-split.md) dividing $b$ and $a^2-4b$, respectively. This [prime-support bound in two-isogeny descent](../../../../../prime-support-bound-in-two-isogeny-descent.md) follows by [valuation](../../../../../valuation.md) comparison: if a [prime](../../../../../prime-number-split.md) does not divide $b$, the [valuations](../../../../../valuation.md) of $x$ at that [prime](../../../../../prime-number-split.md) must be even, whether positive or negative. A candidate squarefree class $d$ is represented precisely when its [quartic covering in a two-isogeny descent](../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
N^2=dU^4+aU^2V^2+(b/d)V^4
$$

has the corresponding rational solution, apart from the separately included identity and two-torsion cases; clearing denominators permits [coprime](../../../../../coprime-integers.md) [integers](../../../../../integer-split.md) $U,V$.

Here $a=5,b=-5$, so

$$
E':Y^2=X(X^2-10X+45).
$$

On $E$ the possible classes are $1,-1,5,-5$. They all occur: the identity gives one, $T=(0,0)$ gives $-5$, and $(-1,3)$ gives $-1$. Since the image is a [group](../../../../../group-split.md), their product also gives five. Thus its image has order four.

On $E'$, the quadratic factor $(X-5)^2+20$ is strictly positive for real $X$. Every nonzero rational $X$-coordinate is therefore positive. The [prime-support bound in two-isogeny descent](../../../../../prime-support-bound-in-two-isogeny-descent.md) restricts its image to $1,3,5,15$. The identity gives one and $(0,0)$ gives $45$, that is class five.

Class three is impossible. Its [quartic covering in a two-isogeny descent](../../../../../quartic-covering-in-a-two-isogeny-descent.md) would require

$$
N^2=3U^4-10U^2V^2+15V^4,\qquad\gcd(U,V)=1.
$$

Modulo three this is $N^2\equiv2U^2V^2$, so three divides $N$ and at least one of $U,V$. They cannot both be divisible. If $3\mid U$ and $3\nmid V$, the right side has [valuation](../../../../../valuation.md) exactly one, from $15V^4$. If $3\mid V$ and $3\nmid U$, it again has [valuation](../../../../../valuation.md) exactly one, from $3U^4$. Either case contradicts its being a square. Class fifteen is then impossible too, since multiplying it by the known image class five would give class three.

Hence the second image is exactly $\{1,5\}$, of order two. The rank formula gives

$$
2^r=\frac{4\cdot2}{4}=2,\qquad\boxed{r=1.}
$$

This proves the [rank-one elliptic curve with coefficients five and minus five](../../../../../rank-one-elliptic-curve-with-coefficients-five-and-minus-five.md) calculation, including the local obstruction that removes the spurious extra descent classes.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
