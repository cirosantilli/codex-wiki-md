<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

To compute the [rank of an elliptic curve](../../../../../rank-of-an-elliptic-curve.md), translate the [rational point](../../../../../rational-point.md) of order two to $(0,0)$ and put the curve in the form $y^2=x^3+ax^2+bx$, with $a,b\in\mathbb Z$ after clearing denominators and $b(a^2-4b)\ne0$. Its two-isogenous partner and the [elliptic isogeny](../../../../../isogeny-of-elliptic-curves.md) are

$$
E':Y^2=X^3-2aX^2+(a^2-4b)X,\qquad
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right).
$$

The maps extend over their exceptional points. The [dual isogeny](../../../../../dual-isogeny.md) is

$$
\widehat\phi(X,Y)=\left(\frac{X-2a+(a^2-4b)/X}{4},\ \frac{Y(1-(a^2-4b)/X^2)}8\right),
\qquad\widehat\phi\phi=[2].
$$

The [two-torsion square-class homomorphism](../../../../../two-torsion-square-class-homomorphism.md) is $\alpha:E(\mathbb Q)\to\mathbb Q^\times/\mathbb Q^{\times2}$, defined by $\alpha(O)=1$, $\alpha((0,0))=[b]$, and $\alpha((x,y))=[x]$ otherwise. Define $\alpha'$ similarly on $E'$ with $b'=a^2-4b$.

Here are the ingredients behind the descent procedure. For a generic chord $y=mx+c$, the cubic of intersection coordinates has root product $c^2$. As the third intersection is the negative of the group sum and negation leaves $x$ unchanged, this proves the square-class [homomorphism](../../../../../homomorphism.md) property. For a line through $(0,0)$, the two nonzero intersection coordinates have product $b$, so the assigned class $[b]$ gives the same multiplicativity. A vertical line has two equal coordinates and contributes their square, and $O$ has identity class. These observations also cover tangencies and the exceptional sums. Its kernel is $\widehat\phi(E'(\mathbb Q))$. Indeed, the displayed formula gives $x(\widehat\phi(X,Y))=(Y/(2X))^2$. Conversely, if a point on $E$ has $x=r^2\ne0$, the possible preimage coordinates satisfy

$$
X^2+(-2a-4r^2)X+(a^2-4b)=0.
$$

Its [elliptic-curve discriminant](../../../../../elliptic-curve-discriminant.md) is $16(r^4+ar^2+b)=16y^2/r^2$, a rational square. A root $X$ and $Y=2rX$, with the sign chosen appropriately, give a preimage. The identity is always in the image. The point $(0,0)$ is in the image exactly when $b$ is a square: its nonzero preimage coordinates are $X=a\pm2\sqrt b$, with $Y=0$. Thus the exceptional points satisfy precisely the same kernel statement. Interchanging the curves similarly gives $\ker\alpha'=\phi(E(\mathbb Q))$.

A [prime](../../../../../prime-number.md) not dividing $b$ can occur only with even [valuation](../../../../../valuation.md) in an $x$-coordinate. If its [valuation](../../../../../valuation.md) is positive, the factor $x^2+ax+b$ is a unit and $2v(y)=v(x)$; if negative, $x^2$ dominates that factor and $2v(y)=3v(x)$. Thus [square classes](../../../../../square-class.md) in $\operatorname{im}\alpha$ have signed square-free representatives dividing $b$, giving finitely many candidates. To test a candidate $d$, put $x=d(u/v)^2$ and $y=duN/v^3$. The curve equation becomes

$$
C_d:\quad N^2=du^4+au^2v^2+\frac bdv^4.
$$

A nontrivial rational solution, including the appropriate limiting points, is exactly a realization of the class. Clear denominators and arrange $\gcd(u,v)=1$ for congruence tests. Do the same for $E'$ with $b'$.

The factor in the [two-isogeny rank formula](../../../../../square-class-index-formula-for-two-isogeny-descent.md) can also be checked directly. Let $A=E(\mathbb Q)$, $B=E'(\mathbb Q)$ and $t=\#A[2]$. The index of $\widehat\phi(B)$ in $A$ is $\#\operatorname{im}\alpha$, while the map from $B/\phi(A)$ onto $\widehat\phi(B)/2A$ has kernel

$$
\ker\widehat\phi/(\ker\widehat\phi\cap\phi(A)).
$$

The numerator has order two. Moreover $\ker\widehat\phi\cap\phi(A)=\phi(A[2])$, since $\widehat\phi\phi P=2P$, and the latter has order $t/2$. Hence this quotient has order $4/t$, and

$$
[A:2A]=\frac{\#\operatorname{im}\alpha\;\#\operatorname{im}\alpha'}{4/t}.
$$

The [Mordell-Weil theorem](../../../../../mordell-weil-group.md) gives $[A:2A]=2^rt$, where $r$ is the rank. Cancelling $t$ yields

$$
\boxed{2^r=\frac{\#\operatorname{im}\alpha\;\#\operatorname{im}\alpha'}4.}
$$

In practice, local congruence and real-solubility tests remove many candidate quartics, giving an upper bound, while [rational point](../../../../../rational-point.md) searches realize classes and give a lower bound. These often coincide. Local solubility alone is not a proof of a [rational point](../../../../../rational-point.md): an everywhere locally soluble covering can still fail globally, so a remaining gap must be reported rather than treated as an exact rank.

For the curve at hand, $a=8$, $b=-7$, $b'=92$, and

$$
E':Y^2=X^3-16X^2+92X.
$$

The first image is contained in $\{1,-1,7,-7\}$ and contains $1,-7$, the latter from the point $(0,0)$. To exclude $-1$, its quartic would require coprime $u,v$ with

$$
N^2=-u^4+8u^2v^2+7v^4.
$$

Modulo $16$, an odd fourth power is $1$ and an even fourth power is $0$. If $u$ is odd and $v$ even the right side is $15$; if $u$ is even and $v$ odd it is $7$; if both are odd it is $14$. None is among the square residues $0,1,4,9$. Thus $-1$ is impossible. The image is a subgroup, so $7$ is also impossible: its product with the known class $-7$ would be $-1$. We obtain $\operatorname{im}\alpha=\{1,-7\}$.

For $E'$, its quadratic factor is $X^2-16X+92=(X-8)^2+28>0$. Every nonzero rational $X$-coordinate is therefore positive. [Prime](../../../../../prime-number.md) support leaves only $1,2,23,46$ as possible classes; $1$ and $23=[92]$ are supplied by $O$ and the two-torsion point. The explicit point $(18,48)$ is on $E'$ because

$$
18^3-16\cdot18^2+92\cdot18=2304=48^2.
$$

Its class is $[18]=2$. Multiplying classes supplies $46$, so $\operatorname{im}\alpha'=\{1,2,23,46\}$. The [two-isogeny rank formula](../../../../../square-class-index-formula-for-two-isogeny-descent.md) now proves

$$
\boxed{2^r=\frac{2\cdot4}4=2,\qquad\operatorname{rank}E(\mathbb Q)=1.}
$$

As an additional concrete point on the original curve, the [dual isogeny](../../../../../dual-isogeny.md) sends $(18,48)$ to $(16/9,116/27)$. The descent calculation proves the rank; it does not by itself certify that this point generates the full free quotient.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
