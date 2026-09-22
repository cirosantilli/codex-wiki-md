<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Complete the square-class map at the identity by $q(O)=1$; at the finite point $T=(0,0)$ its value is the class of $b$. For another [rational point](../../../../rational-point.md) write

$$
x=r/s^2,\qquad y=t/s^3,\qquad\gcd(r,s)=1.
$$

These denominator powers follow because a negative valuation of $x$ forces the leading cubic term to dominate, so that valuation is even and the valuation of $y$ is three halves of it. The equation gives

$$
t^2=r(r^2+ars^2+bs^4).
$$

If a prime $\ell\nmid b$ divides $r$, it does not divide the second factor, since $\ell\nmid s$. Thus $v_\ell(r)$ is even. All denominator valuations are even too. Every image class therefore has a representative which is a signed squarefree divisor of $b$, proving that $\operatorname{im}q$ is finite.

Use the standard 2-isogeny with [kernel](../../../../kernel-of-a-linear-map-split.md) $\{O,T\}$ and [dual isogeny](../../../../dual-isogeny.md) satisfying $\widehat\phi\phi=[2]$, $\phi\widehat\phi=[2]$. Away from the exceptional points one may take

$$
\phi(x,y)=\left(x+a+\frac bx,\ y\left(1-\frac b{x^2}\right)\right).
$$

Applying the analogous isogeny to $E'$ gives a curve with coefficients $4a,16b$; scaling its coordinates by $1/4,1/8$ gives the dual map back to $E$. The analogous descent map $q'$ on $D$ has [kernel](../../../../kernel-of-a-linear-map-split.md) $\phi(C)$ and finite image. The sequence

$$
D/\phi(C)\ \xrightarrow{\widehat\phi}\ C/2C\longrightarrow C/\widehat\phi(D)\longrightarrow0
$$

is exact at the last two terms. Its outside groups are finite, identified with the two finite descent images, so **$C/2C$ is finite**.

For $E_p:y^2=x(x^2-p^2)$, the rational [2-torsion](../../../../2-torsion.md) is $O,(0,0),(p,0),(-p,0)$, of order four. The first descent image is exactly $\{1,-1,p,-p\}$: these classes occur on the [2-torsion](../../../../2-torsion.md), and the divisor-support bound permits no others. The isogenous curve is $E'_p:y^2=x(x^2+4p^2)$. Its real points have $x\ge0$, so the second image lies in the four positive classes $\{1,2,p,2p\}$.

Here the [kernel](../../../../kernel-of-a-linear-map-split.md) $\{O,(0,0)\}$ of the dual is contained in $\phi(C)$, since $\phi(\pm p,0)=(0,0)$. Thus the displayed map $D/\phi(C)\to C/2C$ is injective, and exactness gives

$$
|C/2C|=|\operatorname{im}q|\,|\operatorname{im}q'|=4|\operatorname{im}q'|.
$$

The allowed rank formula makes the left side $2^{R+2}$, so

$$
\boxed{2^R=|\operatorname{im}q'|\le4,\qquad R\le2.}
$$

Now consider the quartic relation. Normalize a nontrivial [integer](../../../../integer-split.md) solution so that $p$ does not divide both $x,y$, by dividing them by $p$ and $z$ by $p^2$ whenever necessary. If $p\nmid x$, reduction modulo $p$ gives $x^4=2z^2$, with $z\ne0$ modulo $p$, making $2$ a [quadratic residue](../../../../quadratic-residue-split.md). If $p\mid x$, then $p\nmid y$ and $p\mid z$; write $x=pX$, $z=pZ$, divide by $p^2$, and reduce to get $y^4=2Z^2$ modulo $p$. Again $2$ is a square. Therefore

$$
\boxed{\left(\frac2p\right)=1,\qquad p\equiv\pm1\pmod8.}
$$

If the class $2$ occurred in $\operatorname{im}q'$, write the corresponding coordinate as $x'=2u^2/v^2$. The curve equation then gives

$$
u^4+p^2v^4=2z^2,\qquad z=\frac{y'v^3}{4u}.
$$

Here $u,v$ are nonzero coprime integers and $z$ is rational. Since $2z^2$ is an [integer](../../../../integer-split.md), its reduced denominator must be one, so $z$ is an [integer](../../../../integer-split.md) too. For $p\equiv3,5\pmod8$ this contradicts the quartic obstruction. Hence class $2$ is absent. A [subgroup](../../../../subgroup.md) of $\{1,2,p,2p\}$ omitting $2$ has order at most two, so $2^R\le2$ and $R\le1$.

For $p=5$, direct substitution verifies the nonintegral point

$$
\boxed{(x,y)=\left(\frac{25}{4},\frac{75}{8}\right).}
$$

A rational torsion point would have integral coordinates by the preceding theorem, so this point has infinite order. Thus $R\ge1$, and together with the upper bound,

$$
\boxed{\operatorname{rank}E_5(\mathbb Q)=1.}
$$

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
