<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [rational point](../../../../../rational-point.md) of order $2$ can be moved to $(0,0)$, giving an integral model

$$
E:y^2=x(x^2+ax+b),\qquad b(a^2-4b)\ne0.
$$

Its [two-isogeny descent](../../../../../two-isogeny-descent.md) partner and the [two-isogeny formula](../../../../../two-isogeny-formula.md) are

$$
E':Y^2=X(X^2-2aX+b'),\qquad b'=a^2-4b,
$$



$$
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),\qquad
\widehat\phi(X,Y)=\left(\frac{X-2a+b'/X}{4},\ \frac{Y(1-b'/X^2)}8\right).
$$

The maps extend over the identity and $(0,0)$, have these two points as their respective kernels, and direct substitution and the doubling formula give $\widehat\phi\phi=[2]$ and $\phi\widehat\phi=[2]$.

Define the [two-torsion square-class homomorphisms](../../../../../two-torsion-square-class-homomorphism.md) by

$$
\alpha:E(\mathbb Q)\longrightarrow\mathbb Q^\times/(\mathbb Q^\times)^2,\qquad
\alpha(O)=1,\quad\alpha((0,0))=b,\quad\alpha((x,y))=x,
$$

and similarly $\alpha'$ for $E'$, using $b'$. To see the homomorphism property, intersect a line $y=mx+c$ with $E$. Its three $x$-coordinates have product $c^2$, since the resulting monic cubic has constant term $-c^2$. The third point is the negative of the sum of the first two, and negation preserves $x$, so the [square classes](../../../../../square-class.md) multiply as required. If the line passes through $(0,0)$, the other two coordinates have product $b$, giving exactly the prescribed exceptional value. Vertical lines and repeated intersections give the identity and tangent cases.

We also verify the kernel needed for descent:

$$
\ker\alpha=\widehat\phi E'(\mathbb Q),\qquad\ker\alpha'=\phi E(\mathbb Q).
$$

For a point on $E'$, the first coordinate of its image under $\widehat\phi$ is $Y^2/(4X^2)$, a square. Conversely, if $P=(s^2,y)$ has square $x$-coordinate, solving $x(\widehat\phi(X,Y))=s^2$ gives

$$
X^2-(2a+4s^2)X+b'=0.
$$

Its [discriminant](../../../../../discriminant.md) is $16(s^4+as^2+b)=(4y/s)^2$, so it has rational nonzero roots $X=a+2s^2\pm2y/s$. Taking $Y=\pm2sX$ gives a point on $E'$; choose the signs so its image has second coordinate $y$. The exceptional point $(0,0)$ lies in the image exactly when $b$ is a square, as seen from the points with $Y=0$, $X=a\pm2\sqrt b$. This proves the first kernel formula. Applying the same argument to $E'$ and then rescaling the second partner by $(X,Y)\mapsto(X/4,Y/8)$ proves the second.

There are only finitely many candidate [square classes](../../../../../square-class.md). For a [rational point](../../../../../rational-point.md) write $x=M/e^2$ and $y=N/e^3$, with $\gcd(M,e)=1$. These denominator forms follow because a negative [prime](../../../../../prime-number.md) [valuation](../../../../../valuation.md) of $x$ makes the leading cubic term the unique lowest-valuation term, forcing that [valuation](../../../../../valuation.md) to be even. Then

$$
N^2=M(M^2+aMe^2+be^4).
$$

If a [prime](../../../../../prime-number.md) divides $M$ but not $b$, the second factor is a [unit](../../../../../unit-in-a-ring.md) at that [prime](../../../../../prime-number.md), so its [valuation](../../../../../valuation.md) in $M$ is even. Thus every class in $\alpha(E)$ has a signed squarefree representative $d\mid b$. This is the [prime-support bound in two-isogeny descent](../../../../../prime-support-bound-in-two-isogeny-descent.md); the analogous candidates for $\alpha'(E')$ divide $b'$.

The class $d$ is realized by a nonexceptional [rational point](../../../../../rational-point.md) precisely when its [quartic covering in a two-isogeny descent](../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
N^2=dU^4+aU^2V^2+(b/d)V^4
$$

has a [rational point](../../../../../rational-point.md) with $UV\ne0$. Indeed substitution $x=d(U/V)^2$, $y=dUN/V^3$ gives the original equation, and conversely the square-class condition gives these parameters. Clearing denominators permits $U,V,N$ integral with $\gcd(U,V)=1$. The zero-coordinate cases account for the already known identity and two-torsion classes.

For clarity, the [two-isogeny rank formula](../../../../../square-class-index-formula-for-two-isogeny-descent.md) contains a factor $4$, even when $E$ has full rational two-torsion. Put $t=\#E(\mathbb Q)[2]$, which is $2$ or $4$, and let $r$ be the rank. From the two kernel formulas and $2E=\widehat\phi\phi E$,

$$
[E:2E]=\frac{\#\alpha(E)\,\#\alpha'(E')}{\delta},\qquad
\delta=[\ker\widehat\phi:\ker\widehat\phi\cap\phi E].
$$

Indeed the kernel of the induced map $E'/\phi E\to\widehat\phi E'/2E$ is $\ker\widehat\phi/(\ker\widehat\phi\cap\phi E)$. The intersection is $\phi(E[2])$, of size $t/2$, so $\delta=4/t$. The [Mordell-Weil theorem](../../../../../mordell-weil-group.md) gives $[E:2E]=2^rt$. Therefore

$$
\boxed{2^r=\frac{\#\alpha(E)\,\#\alpha'(E')}4.}
$$

This gives a practical rank procedure. Enumerate the finitely many signed squarefree divisors of $b,b'$, and test their quartics over the reals and [local fields](../../../../../local-field.md) at $2$ and [primes](../../../../../prime-number.md) dividing the relevant coefficients or [elliptic-curve discriminant](../../../../../elliptic-curve-discriminant.md). These necessary local conditions give finite [Selmer group of an elliptic curve](../../../../../n-selmer-group.md) upper bounds. Search the remaining coverings for [rational points](../../../../../rational-point.md), or search the curves directly, to realize [square classes](../../../../../square-class.md) and obtain lower bounds. One can also exhibit independent points and check independence by the [canonical height pairing](../../../../../canonical-height-pairing.md). When the upper and lower bounds agree, the rank is determined. Local solubility alone does not guarantee a [rational point](../../../../../rational-point.md), so a persistent gap can reflect a nontrivial [Tate–Shafarevich group](../../../../../tate-shafarevich-group.md) rather than a missing congruence test.

Now take $a=0$, $b=-p^2$ for an odd [prime](../../../../../prime-number.md) $p$. The curve has four rational two-torsion points $O,(0,0),(p,0),(-p,0)$. Their images under $\alpha$ are $1,-1,p,-p$. The prime-support bound allows no other classes, so

$$
\alpha(E_p)=\{1,-1,p,-p\},\qquad\#\alpha(E_p)=4.
$$

Its partner is $E'_p:Y^2=X^3+4p^2X$. Any nonidentity [rational point](../../../../../rational-point.md) with $X\ne0$ has $X>0$, because $X^2+4p^2>0$. Also the exceptional point has [square class](../../../../../square-class.md) $4p^2=1$. Thus its image is contained in the four positive candidate classes $\{1,2,p,2p\}$. The [rank bound for a prime congruent-number elliptic curve](../../../../../rank-bound-for-a-prime-congruent-number-elliptic-curve.md) follows:

$$
\boxed{2^{\operatorname{rank}E_p(\mathbb Q)}=\#\alpha'(E'_p)\le4,\qquad\operatorname{rank}E_p(\mathbb Q)\le2.}
$$

For an exact rank-one example, take $p=5$. The point $(X,Y)=(5,25)$ on $E'_5:Y^2=X^3+100X$ realizes the class $5$. The [five-adic obstructions for the congruent-number isogeny covers](../../../../../five-adic-obstructions-for-the-congruent-number-isogeny-covers.md) exclude the other two possible nontrivial classes. For $d=2$, the quartic is

$$
N^2=2U^4+50V^4,\qquad\gcd(U,V)=1.
$$

Modulo $5$, if $5\nmid U$ the right side is $2$, a nonsquare. Hence $U=5U_1$ and $N=5N_1$; primitivity gives $5\nmid V$. Dividing by $25$ then gives $N_1^2=50U_1^4+2V^4\equiv2\pmod5$, again impossible. For $d=10$, the quartic is $N^2=10(U^4+V^4)$. At least one of $U,V$ is nonzero modulo $5$, and their fourth powers are $0$ or $1$, so their sum is $1$ or $2$ modulo $5$. The right side has five-adic [valuation](../../../../../valuation.md) $1$, impossible for a square. Thus $\alpha'(E'_5)=\{1,5\}$ exactly, and

$$
\boxed{p=5,\qquad\operatorname{rank}E_5(\mathbb Q)=1.}
$$

The [dual isogeny](../../../../../dual-isogeny.md) maps $(5,25)$ to $(25/4,-75/8)$ on $E_5$, giving an explicit [rational point](../../../../../rational-point.md) associated with this rank-one computation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
