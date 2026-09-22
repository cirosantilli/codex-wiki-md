<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Translate the [rational point](../../../../../rational-point.md) of order two to $T=(0,0)$ and clear denominators to obtain an integral equation

$$
E:y^2=x^3+ax^2+bx,\qquad b(a^2-4b)\ne0.
$$

The [two-isogeny formula](../../../../../two-isogeny-formula.md) gives

$$
E':Y^2=X^3-2aX^2+(a^2-4b)X,
$$

with $\phi:E\to E'$ and its dual $\widehat\phi:E'\to E$. One choice of signs is

$$
\begin{aligned}
\phi(x,y)&=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right),\\
\widehat\phi(X,Y)&=\left(\frac{X-2a+(a^2-4b)/X}{4},\ \frac{Y(1-(a^2-4b)/X^2)}8\right).
\end{aligned}
$$

These extend across their displayed poles as isogenies; their composition is $[2]$ and their kernels are the respective [rational points](../../../../../rational-point.md) of order two.

The [two-isogeny descent](../../../../../two-isogeny-descent.md) maps into [square classes](../../../../../square-class.md) are

$$
\alpha(O)=1,\quad\alpha(T)=b,\quad\alpha(x,y)=x\pmod{\mathbb Q^{\times2}},
$$

and the analogous map $\alpha'$ on $E'$ uses $a^2-4b$ at its point $(0,0)$. They are homomorphisms, with kernels $\widehat\phi(E'(\mathbb Q))$ and $\phi(E(\mathbb Q))$. For instance the product of the three intersection $x$-coordinates of a chord is the square of its intercept, proving the square-class addition rule; the values at exceptional points come from the same rule or from the divisor $\operatorname{div}(x)=2(T)-2(O)$. This also identifies the maps as the Kummer maps for the two isogenies.

The [square-class index formula for two-isogeny descent](../../../../../square-class-index-formula-for-two-isogeny-descent.md) is

$$
\boxed{2^r=\frac{|\alpha(E(\mathbb Q))|\,|\alpha'(E'(\mathbb Q))|}{4},}
$$

where $r$ is the rank. To see the torsion correction explicitly, put $T'=(0,0)$ on $E'$. Factoring multiplication by two gives

$$
[E:2E]=[E:\widehat\phi E']\,[\widehat\phi E':\widehat\phi\phi E]
=\frac{|\alpha(E)|\,|\alpha'(E')|}{[\langle T'\rangle:\langle T'\rangle\cap\phi E]}.
$$

The last denominator is $4/|E(\mathbb Q)[2]|$: $T'$ is in $\phi E$ exactly when the two additional [torsion points of an elliptic curve](../../../../../torsion-point-of-an-elliptic-curve.md) of order two on $E$ are rational. Since $[E:2E]=2^r|E(\mathbb Q)[2]|$, cancellation gives the formula in both the single and full rational two-torsion cases.

For computing the images, [unit square-class bound for two-isogeny descent](../../../../../unit-square-class-bound-for-two-isogeny-descent.md) restricts $\alpha$ to signed squarefree divisors of $b$, and $\alpha'$ to those of $a^2-4b$. To justify the prime support, negative valuations of a rational $x$-coordinate are even; at a prime not dividing $b$, a positive valuation of $x$ makes $x^2+ax+b$ a unit, so the equation again forces the valuation to be even. A candidate $d$ occurs precisely when the [quartic covering in a two-isogeny descent](../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
N^2=dU^4+aU^2V^2+(b/d)V^4
$$

has a [rational point](../../../../../rational-point.md), with the limiting points at $U=0$ or $V=0$ included. Clearing denominators gives integers with $\gcd(U,V)=1$. For $UV\ne0$, the associated point is $x=d(U/V)^2$, $y=dUN/V^3$. Test these finitely many coverings over $\mathbb R$ and over relevant $\mathbb Q_q$ to eliminate impossible classes; surviving locally soluble classes give an upper bound. Finding [rational points](../../../../../rational-point.md) on them proves membership and often makes the bound exact. Local solubility alone need not prove global solubility, so one must retain the possible Selmer obstruction.

For the illustration take

$$
E_p:y^2=x^3-p^2x,\qquad E'_p:Y^2=X^3+4p^2X,
$$

with $p\equiv3\pmod8$. On $E_p$ all possible [square classes](../../../../../square-class.md) are $1,-1,p,-p$. They all occur: $O$ supplies $1$ and the three points with $y=0$, at $x=0,p,-p$, supply $-1,p,-p$. Hence **$|\alpha(E_p)|=4$**.

On $E'_p$, a nonzero real point has $X>0$, because $X(X^2+4p^2)=Y^2$. Thus only $d=1,2,p,2p$ need be considered, and $d=1$ occurs already at $O$. The other three classes are excluded as follows.

For $d=p$, the covering is $N^2=p(U^4+4V^4)$. Reducing modulo $p$ forces $p\mid N$ and $U^4+4V^4\equiv0$. If $V$ were divisible by $p$, then $U$ would be too, contradicting primitivity. Otherwise $(U^2/(2V^2))^2\equiv-1\pmod p$, impossible since $p\equiv3\pmod4$. For $d=2p$, the equation is $N^2=2p(U^4+V^4)$, which similarly forces $(U^2/V^2)^2\equiv-1\pmod p$. Thus neither class occurs. These are [odd-prime obstructions for the congruent-number isogeny coverings](../../../../../odd-prime-obstructions-for-the-congruent-number-isogeny-coverings.md).

For $d=2$, the equation is $N^2=2(U^4+p^2V^4)$. If exactly one of $U,V$ is odd, its right side is $2\pmod8$, not a square. If both are odd, their fourth powers are $1\pmod{16}$ and $p^2\equiv9\pmod{16}$; hence the right side is $20\pmod{32}$, also not a square. Both even is forbidden by primitivity. This is the [modulo-thirty-two obstruction for a congruent-number descent class](../../../../../modulo-thirty-two-obstruction-for-a-congruent-number-descent-class.md). Consequently **$|\alpha'(E'_p)|=1$**, and the rank formula gives

$$
\boxed{\operatorname{rank}E_p(\mathbb Q)=0.}
$$

To complete the congruent-number conclusion, also determine torsion. At a good prime $q\equiv3\pmod4$, the character sum for $x^3-p^2x$ cancels in pairs $x,-x$, so $\#E_p(\mathbb F_q)=q+1$. Rational torsion injects into good reduction at every odd prime, by the formal kernel, which is a [torsion-free group](../../../../../torsion-free-group.md). If $p\ne3$, use $q=3,7$ to bound its order by $\gcd(4,8)=4$. If $p=3$, use $q=7,11$, giving $\gcd(8,12)=4$. The three [rational points](../../../../../rational-point.md) of order two already give four points, so **$E_p(\mathbb Q)\cong(\mathbb Z/2\mathbb Z)^2$**. This is [rational torsion of a congruent number curve](../../../../../rational-torsion-of-a-congruent-number-curve.md) in the present cases.

A [congruent number](../../../../../congruent-number.md) is the positive area of a [right triangle](../../../../../right-triangle.md) with rational side lengths. A point $(x,y)$ on $E_p$ with $y\ne0$ would give such a triangle with sides

$$
A=\left|\frac{x^2-p^2}{y}\right|,\quad B=\left|\frac{2px}{y}\right|,\quad C=\left|\frac{x^2+p^2}{y}\right|,
$$

for which $A^2+B^2=C^2$ and $AB/2=p$. Conversely a rational [right triangle](../../../../../right-triangle.md) of area $p$ gives a point with nonzero $y$, for example $x=p(C+A)/B$, $y=2p^2(C+A)/B^2$. But every [rational point](../../../../../rational-point.md) on the curve just determined is $O$ or has $y=0$. **Every prime $p\equiv3\pmod8$ is therefore not a congruent number.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
