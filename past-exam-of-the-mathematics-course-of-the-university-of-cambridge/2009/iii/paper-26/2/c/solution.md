<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We first determine the torsion. The rational [2-torsion](../../../../../../2-torsion.md) points are $O,(0,0),(5,0),(-5,0)$. At the good primes three and seven, part (b) gives group orders four and eight. Prime-to-residue-characteristic torsion injects under reduction: an element in the kernel has a formal parameter $t$ of positive valuation, and multiplication by an integer prime to the residue characteristic has series $mt+O(t^2)$ with unit leading coefficient, so cannot kill a nonzero such parameter. At seven this excludes rational 3-primary torsion; at three it excludes 7-primary torsion and every odd-primary component other than the already excluded 3-primary component. Thus all torsion is 2-primary and injects at three, bounding its order by four. Consequently

$$
E_5(\mathbb Q)_{\mathrm{tors}}=\{O,(0,0),(5,0),(-5,0)\}\cong(\mathbb Z/2\mathbb Z)^2.
$$

For the rank, use [two-isogeny descent](../../../../../../two-isogeny-descent.md) with

$$
E:y^2=x^3-25x,\qquad E':Y^2=X^3+100X.
$$

The [two-isogeny formula](../../../../../../two-isogeny-formula.md) gives

$$
\phi(x,y)=\left(x-\frac{25}{x},\ y\left(1+\frac{25}{x^2}\right)\right),\qquad
\psi(X,Y)=\left(\frac{Y^2}{4X^2},\ \frac{Y}{8}\left(1-\frac{100}{X^2}\right)\right).
$$

They extend at the exceptional points, have kernels $\{O,(0,0)\}$ on their respective curves, and satisfy $\psi\phi=[2]$. These assertions can be checked by substitution; for example the composed x-coordinate is $(x^2+25)^2/[4x(x^2-25)]$, the duplication x-coordinate. The maps respect addition because they are morphisms fixing $O$: pushforward of [divisor classes](../../../../../../divisor-class.md) is additive, takes [principal divisors](../../../../../../principal-divisor-on-an-algebraic-curve.md) to [principal divisors](../../../../../../principal-divisor-on-an-algebraic-curve.md) by the norm of a rational function, and under the identification in part 1(a) sends $[(P)-(O)]$ to $[(\phi P)-(O)]$, and likewise for $\psi$.

Define the [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md) $\alpha:E(\mathbb Q)\to\mathbb Q^\times/\mathbb Q^{\times2}$ by $\alpha(x,y)=[x]$, $\alpha(O)=1$, and $\alpha((0,0))=[-25]=[-1]$. Define $\alpha'$ on $E'$ similarly, with $\alpha'((0,0))=[100]=1$. To see the homomorphism property, a nonvertical line $y=mx+c$ cuts either curve in three points whose x-coordinates have product $c^2$. The chord-and-tangent law therefore makes their square classes multiply to one. When the line passes through $(0,0)$, the two remaining x-coordinates have product equal to the coefficient of $x$, exactly explaining the assigned value there. Vertical lines give the inverse-point relation. The same argument includes repeated tangent intersections.

The kernels are $\ker\alpha=\psi E'(\mathbb Q)$ and $\ker\alpha'=\phi E(\mathbb Q)$. Here is an explicit check, not just an invocation of the descent correspondence. The x-coordinate of every nonexceptional $\psi$-image is a square. Conversely, if $(x,y)\in E$ has $x=s^2\ne0$, put $X=2x+2y/s$ and $Y=2sX$. Then $X^2-4xX+100=0$, so $(X,Y)\in E'$ and the displayed $\psi$ maps it to $(x,y)$. For $E'$, every nonexceptional $\phi$-image has $X=(y/x)^2$; if $X=s^2\ne0$, put $x=(X+Y/s)/2$, $y=sx$. Substitution gives a point of $E$ mapping to $(X,Y)$. The point $(0,0)\in E'$ has square class one and equals $\phi(5,0)$; the point $(0,0)\in E$ has nonsquare class $-1$. Together with the origins these checks handle every exception.

The [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md) can be read directly from $y^2=x(x^2+B)$. At a prime not dividing the integral coefficient $B$, positive valuation of $x$ gives $2v(y)=v(x)$, while negative valuation gives $2v(y)=3v(x)$; either way the valuation of $x$ is even. Thus the first image has only the candidate classes $1,-1,5,-5$. All four occur, already at the four torsion points. Hence $\#\alpha(E)=4$.

On $E'$, nonzero real x-coordinates are positive since $X(X^2+100)$ has the sign of $X$. Prime support leaves only $1,2,5,10$. The point $(5,25)$ supplies class five. Class two would give the [quartic covering in a two-isogeny descent](../../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
W^2=2U^4+50V^4,\qquad\gcd(U,V)=1.
$$

Indeed write $X=2(U/V)^2$ and clear the square factor in the curve equation. If $5\nmid U$, the right side is two modulo five, impossible for a square. If $5\mid U$, then $5\nmid V$ and $5\mid W$; division by twenty-five gives $(W/5)^2\equiv2V^4\equiv2\pmod5$, again impossible. This is the [five-adic obstruction to square class two on the curve with coefficient one hundred](../../../../../../five-adic-obstruction-to-square-class-two-on-the-curve-with-coefficient-one-hundred.md). Because the image is a subgroup and contains five, class ten is excluded as well. Therefore $\alpha'(E')=\{1,5\}$ has size two.

Now $[E:\psi E']=4$. The quotient $\psi E'/2E$ is isomorphic to $E'/\phi E$: the kernel of the induced surjection is $\ker\psi/(\ker\psi\cap\phi E)$, which is trivial because $(0,0)\in E'$ equals $\phi(5,0)$. Thus $[E:2E]=4\cdot2=8$. Finite generation follows from the [Mordell-Weil theorem](../../../../../../mordell-weil-group.md), whose height-descent proof is supplied in the essay below. A finitely generated group with the torsion already found has $[E:2E]=2^{r+2}$, so $r=1$. Hence

$$
\boxed{E_5(\mathbb Q)\cong(\mathbb Z/2\mathbb Z)^2\times\mathbb Z.}
$$

The point $(-4,6)$ has infinite order, since it is not one of the torsion points. No assertion that this particular point generates the free factor is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
