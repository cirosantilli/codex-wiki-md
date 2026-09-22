<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [elliptic-curve discriminant](../../../../../elliptic-curve-discriminant.md) of $y^2=x^3-12x^2+20x$ is $16\cdot20^2\cdot(144-80)=409600=2^{14}5^2$. Thus three and eleven are primes of [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md). Counting the reduced points gives four points over $\mathbb F_3$ and sixteen over $\mathbb F_{11}$. For example, the numbers of affine points above successive $x=0,1,2$ modulo three are $1,1,1$. Modulo eleven, for $x=0,\ldots,10$, they are $1,2,1,2,0,0,2,2,2,2,1$; add the point at infinity in each case.

The [reduction of torsion points on an elliptic curve](../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) is injective on torsion prime to the residue characteristic. The three-primary rational torsion injects into the group of order sixteen at eleven, so is trivial; likewise the eleven-primary torsion injects into the group of order four at three. Every other primary component injects at both primes. Therefore the rational [torsion subgroup](../../../../../torsion-subgroup.md) has order dividing four. All four rational [2-torsion](../../../../../2-torsion.md) points are visible, so

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\{O,(0,0),(2,0),(10,0)\}\cong(\mathbb Z/2\mathbb Z)^2.}
$$

The rational point $P=(1,3)$ lies on the curve. The tangent slope in the [elliptic-curve addition formula](../../../../../elliptic-curve-addition-formula.md) is $(3-24+20)/6=-1/6$, giving $2P=(361/36,-323/216)$. The integral substitution $X=x-4$ changes the equation to $y^2=X^3-28X-48$; the doubled point has $X=217/36$. The [Nagell–Lutz theorem](../../../../../nagell-lutz-theorem.md) says that a rational torsion point on this integral short equation has integral coordinates, so $2P$, and hence $P$, is nontorsion. **An infinite-order point is $(1,3)$.**

We prove the rank bound by [two-isogeny descent](../../../../../two-isogeny-descent.md). For $a=-12,b=20$, the [two-isogeny formula](../../../../../two-isogeny-formula.md) gives the partner

$$
E':Y^2=X^3+24X^2+64X
$$

and maps $\phi:E\to E'$, $\psi:E'\to E$ with $\psi\phi=[2]$. The [two-torsion square-class homomorphism](../../../../../two-torsion-square-class-homomorphism.md) $\alpha:E(\mathbb Q)\to\mathbb Q^*/(\mathbb Q^*)^2$ is $\alpha(x,y)=[x]$ away from $O,(0,0)$, with values $1$ and $[20]=[5]$ at those exceptional points. Its kernel is $\psi E'(\mathbb Q)$. The corresponding map $\alpha'$ on $E'$ has kernel $\phi E(\mathbb Q)$.

The [prime-support bound in two-isogeny descent](../../../../../prime-support-bound-in-two-isogeny-descent.md) can be checked directly here. For a prime $\ell\nmid20$, if $v_\ell(x)>0$ then $x^2-12x+20$ is a unit, so $2v_\ell(y)=v_\ell(x)$ is even; if $v_\ell(x)<0$, the $x^3$ term has strictly least valuation and $2v_\ell(y)=3v_\ell(x)$ is even. Thus the square class of $x$ is supported only on two and five. Also $x(x-2)(x-10)\geq0$ forces $x\in[0,2]\cup[10,\infty)$, so nonzero $x$ is positive. The possible classes are $1,2,5,10$, and the four torsion points provide all of them:

$$
\alpha(O)=1,\quad\alpha((2,0))=2,\quad
\alpha((0,0))=5,\quad\alpha((10,0))=10.
$$

Consequently $\#\alpha(E(\mathbb Q))=4$.

The same valuation argument on $E'$ gives possible signed classes $1,-1,2,-2$, since its coefficient $b'=64$ has only the prime two. The identity gives class $1$, and $(-4,8)\in E'(\mathbb Q)$ gives class $-1$. For $d=\pm2$, the [two-isogeny descent quartic](../../../../../quartic-covering-in-a-two-isogeny-descent.md) is

$$
W^2=dU^4+24U^2V^2+(64/d)V^4,
$$

with integral coprime $U,V$ after scaling a rational solution. If $U$ is odd, its right side is $2$ or $10$ modulo sixteen for $d=2$, and $14$ or $6$ for $d=-2$, according to the parity of $V$. None is a square. If $U=2u$ is even, $V$ is odd and the right side is $32(\pm u^4+3u^2V^2\pm V^4)$. The bracket is odd for either parity of $u$, so its [2-adic valuation](../../../../../2-adic-valuation.md) is five, again impossible for a square. The [signed divisor-two obstruction for an isogeny covering](../../../../../signed-divisor-two-obstruction-for-an-isogeny-covering.md) excludes both classes. Hence $\alpha'(E'(\mathbb Q))=\{1,-1\}$.

For completeness, the index correction in the [two-isogeny index formula over a number field](../../../../../two-isogeny-index-formula-over-a-number-field.md) is one: $\ker\psi=\{O,(0,0)\}$ and $\phi((2,0))=(0,0)$, so the whole kernel lies in $\phi E(\mathbb Q)$. Thus

$$
[E(\mathbb Q):2E(\mathbb Q)]=\#\alpha(E(\mathbb Q))\,\#\alpha'(E'(\mathbb Q))=4\cdot2=8.
$$

The [Mordell-Weil theorem](../../../../../mordell-weil-group.md) and the four rational [2-torsion](../../../../../2-torsion.md) points identify this index as $2^{r+2}$. Therefore $2^{r+2}=8$ and

$$
\boxed{\operatorname{rank}E(\mathbb Q)=1.}
$$

This is the [rank-one elliptic curve with roots zero two and ten](../../../../../rank-one-elliptic-curve-with-roots-zero-two-and-ten.md). We have exhibited a point of infinite order but have not needed to prove that it generates the free part.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
