# Paper 125

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_125.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_125.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [smooth projective curve](../../../projective-space.md#smooth-projective-curve) $C$ of [geometric genus](../../../normalization-of-an-algebraic-curve.md#geometric-genus) one, the [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) says

$$
\ell(D)-\ell(K_C-D)=\deg D.
$$

The [canonical divisor](../../../algebraic-geometry.md#canonical-divisor) has degree zero and is principal because a nonzero regular differential has no zeros. Hence $K_C\sim0$, so equivalently

$$
\ell(D)-\ell(-D)=\deg D.
$$

In particular, $\ell(D)=\deg D$ when $\deg D>0$.

The group $\operatorname{Pic}^0(E)$ is the group of degree-zero [divisor classes](../../../algebraic-geometry.md#divisor-class) on $E$, with addition induced by addition of divisors. Consider

$$
\iota:E\longrightarrow\operatorname{Pic}^0(E),
\qquad P\longmapsto[(P)-(O_E)].
$$

For surjectivity, let $D$ have degree zero. Since $\deg(D+(O_E))=1$, Riemann--Roch gives $\ell(D+(O_E))=1$. A nonzero element of this space makes $D+(O_E)$ linearly equivalent to an effective divisor of degree one, necessarily $(P)$ for some point $P$. Thus $[D]=[(P)-(O_E)]$.

For injectivity, suppose $(P)-(O_E)$ is a [principal divisor](../../../algebraic-geometry.md#principal-divisor-on-an-algebraic-curve). If $P\ne O_E$, its defining function would be nonconstant and would have at most one simple pole, whereas Riemann--Roch gives $\ell((O_E))=1$, so every such function is constant. Therefore $P=O_E$, and $\iota$ is a bijection.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Embed $E$ as a smooth plane cubic with $O_E$ an [inflection point](../../../normalization-of-an-algebraic-curve.md#inflection-point-of-a-plane-cubic). A line through $P,Q$, using the tangent when $P=Q$, has a third intersection $S$ counted with multiplicity. The [chord-and-tangent group law](../../../normalization-of-an-algebraic-curve.md#chord-and-tangent-group-law) defines $P+Q=-S$, where $-S$ is the third point on the line through $S$ and $O_E$.

The divisor cut out by the first line is

$$
(P)+(Q)+(S)-3(O_E),
$$

and the line through $S$ and $O_E$ gives $(S)+(-S)-2(O_E)$. Their quotient therefore shows

$$
[(P)-(O_E)]+[(Q)-(O_E)]=[(P+Q)-(O_E)].
$$

Under the bijection from part (a), the chord-and-tangent operation is exactly addition in the [abelian group](../../../group.md#abelian-group) $\operatorname{Pic}^0(E)$. It is consequently associative and commutative, has identity $O_E$, and has the geometrically defined point $-P$ as inverse. Thus it makes $E$ an abelian group.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Because $\phi$ is a [separable isogeny](../../../normalization-of-an-algebraic-curve.md#separable-isogeny),

$$
\phi^*(O_{E_2})=\sum_{T\in E_1[\phi]}(T).
$$

The degree-zero divisor

$$
D=\phi^*(O_{E_2})-d(O_{E_1})
$$

corresponds under $E_1\simeq\operatorname{Pic}^0(E_1)$ to the sum of all elements of the finite abelian group $E_1[\phi]$. Pairing every $T$ with $-T$ shows that this sum is the sum of the elements in $E_1[\phi]\cap E_1[2]$. It vanishes when that intersection has one element and also when it has four elements, since the sum of the four elements of $(\mathbb Z/2\mathbb Z)^2$ is zero. The [principal divisor criterion on an elliptic curve](../../../algebraic-geometry.md#principal-divisor-criterion-on-an-elliptic-curve) therefore gives a rational function $g$ with $\operatorname{div}(g)=D$.

The divisor $D$ is invariant under $[-1]$, so $[-1]^*g/g$ has zero divisor and is constant. Applying $[-1]$ twice shows that this constant has square one; hence $[-1]^*g=\pm g$.

For a short [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve)

$$
E:y^2=x^3+Ax+B,
$$

the multiplication-by-two isogeny has

$$
\operatorname{div}(y)=\sum_{T\in E[2]}(T)-4(O_E)=[2]^*(O_E)-4(O_E).
$$

Thus one may take $g=y$, and $[-1]^*y=-y$. For multiplication by three, the third [division polynomial of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#division-polynomials)

$$
\psi_3(x)=3x^4+6Ax^2+12Bx-A^2
$$

vanishes simply at the eight nonzero points of $E[3]$ and has a pole of order eight at $O_E$. Hence $g=\psi_3(x)$ has divisor $[3]^*(O_E)-9(O_E)$ and satisfies $[-1]^*g=g$. Both signs occur.

## 2

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Hasse theorem for elliptic curves](../../../normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves) states that for $E/\mathbb F_q$,

$$
\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.
$$

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve). Its fixed points are exactly $E(\mathbb F_q)$, and $1-\pi$ is separable because its differential is the identity. Therefore

$$
\#E(\mathbb F_q)=\#\ker(1-\pi)=\deg(1-\pi).
$$

For every endomorphism $\alpha$, the [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) gives $\alpha\widehat\alpha=[\deg\alpha]$, and the degree satisfies the parallelogram law

$$
\deg(\alpha+\beta)+\deg(\alpha-\beta)=2\deg\alpha+2\deg\beta.
$$

Consequently, if $a=1+q-\deg(1-\pi)$ is the [trace](../../../normalization-of-an-algebraic-curve.md#trace-of-an-elliptic-curve-endomorphism) of $\pi$, then

$$
\deg([m]-[n]\pi)=m^2-amn+qn^2.
$$

This is nonnegative for every pair of integers $m,n$. By approximating the minimizing real ratio $m/n=a/2$, the quadratic polynomial can be nonnegative for all rational ratios only if its discriminant is nonpositive. Thus $a^2\leq4q$, and the displayed point-count identity proves Hasse's theorem.

An explicit example with nonisomorphic groups occurs over $\mathbb F_{43}$. Put

$$
E_1:y^2=x^3+2x+4,
\qquad
E_2:y^2=x^3+20.
$$

On $E_1$, the point $(30,19)$ has order seven and its nonzero cyclic subgroup has $x$-coordinates $30,31,40$. [Vélu formulas](../../../normalization-of-an-algebraic-curve.md#velu-s-formulas) give the quotient coefficients

$$
v=6\sum x_i^2+6A=9,
\qquad
w=10\sum x_i^3+6A\sum x_i+12B=10
\pmod {43},
$$

so the degree-seven quotient is

$$
A'=A-5v=0,
\qquad B'=B-7w=20,
$$

which is $E_2$. Direct quadratic-residue counts give $\#E_1(\mathbb F_{43})=\#E_2(\mathbb F_{43})=49$. The points killed by seven on $E_1$ are only the displayed kernel and $O$, while $(1,8)$ and $(3,2)$ are independent seven-torsion points on $E_2$. Hence

$$
E_1(\mathbb F_{43})\cong\mathbb Z/49\mathbb Z,
\qquad
E_2(\mathbb F_{43})\cong(\mathbb Z/7\mathbb Z)^2.
$$

Finally, let $p<43$ and suppose two curves are linked by an isogeny of degree seven. The isogeny and its dual induce inverse isomorphisms on every prime-to-seven primary subgroup, so nonisomorphic rational point groups would require $49$ to divide their common order. Since this order is less than $57$ by Hasse, one group would then be cyclic of order $49$ and the other would contain all of $E[7]$. The [Weil pairing](../../../normalization-of-an-algebraic-curve.md#weil-pairing) on rational seven-torsion forces $\mu_7\subset\mathbb F_p$, hence $p\equiv1\pmod7$ unless $p=7$. The only prime below $43$ congruent to one modulo seven is $29$, but Hasse gives $\#E(\mathbb F_{29})<49$; for $p=7$ the same inequality is immediate. No such pair exists below $43$.

## 3

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The curve has [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) when it admits a [Minimal Weierstrass equation](../../../normalization-of-an-algebraic-curve.md#minimal-weierstrass-equation) over $\mathcal O_K$ whose discriminant is a unit, so reduction modulo $\pi$ is a nonsingular elliptic curve $\widetilde E/k$. Write a point of $E(K)$ in primitive projective coordinates $(X:Y:Z)$ over $\mathcal O_K$. Reducing all three coordinates defines

$$
\operatorname{red}:E(K)\longrightarrow\widetilde E(k),
\qquad (X:Y:Z)\longmapsto(\widetilde X:\widetilde Y:\widetilde Z).
$$

Primitivity ensures that the reduced triple is not zero. The addition morphism on the smooth Weierstrass model reduces to the addition morphism on $\widetilde E$; equivalently, this follows from the [valuative criterion for properness](../../../ringed-space.md#valuative-criterion-for-properness) for the smooth proper group scheme. Therefore $\operatorname{red}(P+Q)=\operatorname{red}(P)+\operatorname{red}(Q)$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The needed [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) says that if $f\in\mathcal O_K[X]$ and $a\in\mathcal O_K$ satisfy $f(a)\equiv0\pmod\pi$ and $f'(a)\not\equiv0\pmod\pi$, then $a$ lifts uniquely to a root of $f$ in $\mathcal O_K$ with the prescribed residue. At every affine point of the smooth curve $\widetilde E$, one partial derivative of its Weierstrass equation is nonzero. Fixing the other coordinate and applying Hensel's lemma lifts that point to $E(K)$; $O_E$ lifts itself. Thus reduction is surjective.

Use the local parameters

$$
t=-x/y,
\qquad z=-1/y,
$$

so $x=t/z$ and $y=-1/z$. Substitution in a general integral Weierstrass equation gives

$$
z=t^3+a_1tz+a_2t^2z+a_3z^2+a_4tz^2+a_6z^3.
$$

For fixed $0\ne t\in\pi\mathcal O_K$, the difference between the two sides, viewed as a polynomial in $z$, is congruent to $z$ modulo $\pi$ and has derivative congruent to one. Hensel's lemma gives a unique $z\in\pi\mathcal O_K$, and therefore a unique point $\theta(t)=(t/z,-1/z)$ in the [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve). Together with $\theta(0)=O_E$, this identifies that kernel with the parameters $t\in\pi\mathcal O_K$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $K^{\mathrm{nr}}$ be the maximal [unramified extension](../../../arithmetic.md#unramified-extension) of $K$. Because $p\nmid n$, multiplication by $n$ on the special fibre is a separable isogeny and is surjective on $\widetilde E(\overline k)$. Choose a point $\widetilde Q$ with $[n]\widetilde Q=\widetilde P$ and lift it, after a finite unramified extension, to $Q_0$. Then $R=P-[n]Q_0$ lies in the kernel of reduction.

On the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve), multiplication by $n$ has the form

$$
[n]_F(T)=nT+O(T^2).
$$

Since $n$ is a unit in $\mathcal O_K$, the [invertible morphism criterion for formal group laws](../../../normalization-of-an-algebraic-curve.md#invertible-morphism-criterion-for-formal-group-laws) makes $[n]_F$ an automorphism of $\pi\mathcal O_{K^{\mathrm{nr}}}$. Hence $R=[n]S$ for a unique point $S$ in the kernel of reduction, and $Q=Q_0+S$ satisfies $[n]Q=P$. Moreover, good reduction makes the finite group scheme $E[n]$ étale over $\mathcal O_K$, so all its points are defined over an unramified extension. Every point of $[n]^{-1}P=Q+E[n]$ is therefore unramified, proving that $K([n]^{-1}P)/K$ is unramified.

Multiplication by $n$ is already an automorphism of the formal kernel, so the exact reduction sequence shows that $E(K)/nE(K)$ is finite. Choose representatives $P_1,\ldots,P_s$. Each becomes $n$-divisible over a finite unramified extension; their compositum $L/K$ is still finite and unramified. Every class from $E(K)/nE(K)$ then maps to zero in $E(L)/nE(L)$.

## 4

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $x=u/v\in\mathbb Q$ in lowest terms, the [naive height on the projective line](../../../normalization-of-an-algebraic-curve.md#naive-height-on-the-projective-line) is

$$
H(x)=\max\{|u|,|v|\}.
$$

Homogenize the coprime numerator and denominator of $\xi$ to degree $d$. The triangle inequality gives the upper estimate $H(\xi(x))\leq c_2H(x)^d$. Since the two homogenized forms have no common projective zero, their [resultant](../../../polynomial.md#resultant) is nonzero, and the Bézout identities for the resultant express fixed multiples of $u^{2d-1}$ and $v^{2d-1}$ as combinations of their values with coefficients of degree $d-1$. After cancellation this gives $H(x)^d\leq C H(\xi(x))$, which is the lower estimate with $c_1=C^{-1}$.

Now write $x=u/v$ in lowest terms and put

$$
N=u^3+auv^2+bv^3.
$$

Since $\gcd(N,v)=1$, the equation $y^2=N/v^3$ gives

$$
H(y)^2=\max\{|N|,|v|^3\}=:M.
$$

Clearly $M\leq\gamma H(x)^3$ for $\gamma=1+|a|+|b|$. Homogenizing the supplied polynomial identity gives

$$
u^5=(u^2-av^2)N-(bu^2-a^2uv-abv^2)v^3.
$$

Its coefficient sum is at most $\gamma^2$, so $|u|^5\leq\gamma^2H(x)^2M$. The same lower bound is immediate from $|v|^3\leq M$ when $|v|=H(x)$. Thus

$$
\boxed{\gamma^{-2}H(x)^3\leq H(y)^2\leq\gamma H(x)^3.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set $h(O_E)=0$ and

$$
h(P)=\log H(x(P))
$$

for $P\ne O_E$. The [canonical height of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve) is

$$
\widehat h(P)=\frac12\lim_{r\to\infty}4^{-r}h([2^r]P).
$$

The duplication formula is a rational function of degree four in $x$, so the rational-map height estimate in part (a) gives

$$
|h([2]P)-4h(P)|\leq C_E.
$$

Therefore successive terms of $4^{-r}h([2^r]P)$ differ by at most $C_E4^{-r-1}$, and the limit is well defined.

Shifting the limit immediately gives $\widehat h([2]P)=4\widehat h(P)$. The addition formula likewise gives

$$
h(P+Q)+h(P-Q)=2h(P)+2h(Q)+O_E(1).
$$

Apply this to $[2^r]P,[2^r]Q$, divide by $2\cdot4^r$, and pass to the limit to obtain the exact [parallelogram law](../../../linear-algebra.md#parallelogram-law)

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

Taking $Q=P$ starts an induction on $|n|$ that yields

$$
\widehat h([n]P)=n^2\widehat h(P)
$$

for every integer $n$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

An admissible change of [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) replaces the $x$-coordinate by a degree-one rational function, so the two logarithmic heights differ by $O(1)$. Dividing this bounded difference by $4^r$ in the defining limit shows that the canonical height is unchanged. It is intrinsic to the elliptic curve and the chosen point.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Replacing $[2^r]$ and $4^r$ by $[3^r]$ and $9^r$ gives the same canonical height. Indeed $h([3]P)=9h(P)+O_E(1)$, and the same telescoping argument constructs a quadratic height differing from the original by a bounded function. A bounded quadratic function is zero, so the two limits agree.

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Part (a) gives

$$
2\log H(y(P))=3\log H(x(P))+O_E(1).
$$

**Thus replacing the $x$-coordinate height literally by the $y$-coordinate height multiplies the resulting canonical height by $3/2$. Multiplying the new naive height by $2/3$ restores the original normalization.**

## 5

↑ **Parent:** [Paper 125](paper-125.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Fix a prime $p$. If a rational point $T=(x,y)$ has $v_p(x)<0$, the integral projective Weierstrass equation forces

$$
v_p(x)=-2m,
\qquad v_p(y)=-3m
$$

for some $m>0$. Hence its formal parameter $t=-x/y$ lies in $p\mathbb Z_p$, so $T$ belongs to the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve) at the identity. This formal kernel has no nonzero torsion for the present equation. Multiplication by an integer prime to $p$ is a formal-group automorphism, while the [formal logarithm](../../../normalization-of-an-algebraic-curve.md#formal-logarithm) rules out $p$-power torsion for odd $p$. For $p=2$, inversion sends $t$ to $-t$ because the equation has no $xy$ or $y$ term, and therefore

$$
[2]_F(t)=2t+O(t^3).
$$

For $v_2(t)\geq1$, its leading term has strictly smaller valuation than every higher term, so $[2]_F(t)$ cannot vanish; iterating excludes all two-power torsion as well.

Thus a nonzero torsion point cannot have $v_p(x)<0$. Since this holds for every prime, $x\in\mathbb Z$. The integral equation then makes $y^2$ an integer; a rational number whose square is integral is itself integral, so $y\in\mathbb Z$. This is the integrality assertion in the [Lutz–Nagell theorem](../../../normalization-of-an-algebraic-curve.md#nagell-lutz-theorem).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For $E:y^2=x^3-x^2+25x$, the addition formulas give

$$
P+T=(25,-125),
\qquad
Q+T=(5,-15)=-Q,
\qquad
P+Q=(5/4,-45/8).
$$

In particular, $[2]Q=T$ and $Q$ has order four, while the nonintegral coordinate of $[2]P=(144/25,-2172/125)$ and part (a) show that $P$ has infinite order.

For [two-isogeny descent](../../../normalization-of-an-algebraic-curve.md#two-isogeny-descent), write

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

The [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve) injects rational torsion into both groups, so its order divides $\gcd(12,16)=4$. Since $Q$ has order four, the torsion subgroup is $\mathbb Z/4\mathbb Z$. Therefore

$$
E(\mathbb Q)\cong\mathbb Z/4\mathbb Z\times\mathbb Z,
$$

so $t=1$, $d_1=4$, and $r=1$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
