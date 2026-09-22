# Paper 28

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper28.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper28.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Hasse theorem for elliptic curves](../../../normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves) states

$$
\boxed{\left|\#E(\mathbb F_q)-(q+1)\right|\le2\sqrt q.}
$$

We prove it by the positive [degree of an isogeny](../../../normalization-of-an-algebraic-curve.md#degree-of-an-isogeny). Let $\pi$ be the $q$-power [Frobenius isogeny](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve), of degree $q$. Its fixed points are precisely $E(\mathbb F_q)$, so they form the kernel of $1-\pi$. Since the differential of $\pi$ is zero, the differential of $1-\pi$ is the identity; thus $1-\pi$ is a [separable isogeny](../../../normalization-of-an-algebraic-curve.md#separable-isogeny). Its degree is the number of its geometric kernel points. Therefore

$$
N:=\#E(\mathbb F_q)=\deg(1-\pi).
$$

We use the standard [degree parallelogram law](../../../normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law), together with $\deg[m]=m^2$: degree, extended by zero at the zero endomorphism, is a positive [quadratic form](../../../linear-algebra.md#quadratic-form) on the [endomorphism ring of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve). Put $t=1+q-N$, the [Trace of Frobenius](../../../normalization-of-an-algebraic-curve.md#trace-of-frobenius). Polarizing the degree form gives, for every pair of integers $m,n$,

$$
\deg([m]-[n]\pi)=m^2-tmn+qn^2\ge0.
$$

Indeed, the values on $1$ and $\pi$ are $1$ and $q$, and the cross coefficient is fixed by $\deg(1-\pi)=1+q-t$. These are standard degree facts about [isogenies of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves), which suffice without an assumption about characteristic or ordinariness.

For $n\ne0$, division by $n^2$ shows $x^2-tx+q\ge0$ at every rational $x=m/n$. Density of the [rational numbers](../../../number-theory.md#rational-number) and continuity of this polynomial make it nonnegative on the real line. Evaluating at its minimum $x=t/2$ gives $q-t^2/4\ge0$, whence $|t|\le2\sqrt q$. Since $N=q+1-t$, this proves the estimate. This is the [degree-form proof of the Hasse bound](../../../normalization-of-an-algebraic-curve.md#degree-form-proof-of-the-hasse-bound); it proves both sides simultaneously by positivity of one degree form.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $t=q+1-\#E(\mathbb F_q)$. The stated characteristic equation for the [Frobenius isogeny](../../../normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve) is

$$
\pi^2-[t]\pi+[q]=0.
$$

Take $\alpha,\beta$ to be the complex roots of $T^2-tT+q$. They satisfy $\alpha+\beta=t$ and $\alpha\beta=q$. By the [Hasse bound](../../../normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves), $t^2\le4q$. If the inequality is strict, the roots are complex conjugates and have squared modulus $q$. In the equality case both roots are the same real number $\pm\sqrt q$. Thus in every case

$$
|\alpha|=|\beta|=\sqrt q,\qquad \beta=q/\alpha.
$$

To obtain every extension-field count without assuming distinct roots, set $t_n=\operatorname{tr}(\pi^n)$ and $t_0=2$. The [dual isogeny](../../../normalization-of-an-algebraic-curve.md#dual-isogeny) satisfies $\widehat\pi\pi=[q]$ and $\pi+\widehat\pi=[t]$. Consequently the sums $\pi^n+\widehat\pi^{\,n}=[t_n]$ satisfy

$$
t_n=t\,t_{n-1}-q\,t_{n-2},\qquad t_0=2,\quad t_1=t.
$$

Alternatively, apply additivity of the [trace of an elliptic-curve endomorphism](../../../normalization-of-an-algebraic-curve.md#trace-of-an-elliptic-curve-endomorphism) directly to the characteristic equation multiplied by $\pi^{n-2}$. The sequence $\alpha^n+\beta^n$ has the same recurrence and initial values, so $t_n=\alpha^n+\beta^n$ by induction. This is the [Frobenius trace recurrence](../../../normalization-of-an-algebraic-curve.md#frobenius-trace-recurrence), valid also at a repeated root.

The fixed points of $\pi^n$ are $E(\mathbb F_{q^n})$, and $1-\pi^n$ is again separable. Since $\deg\pi^n=q^n$, the trace-degree identity gives

$$
\#E(\mathbb F_{q^n})=\deg(1-\pi^n)=1+q^n-t_n
=1+q^n-\alpha^n-\beta^n.
$$

Factoring and using $\beta=q/\alpha$ yields

$$
\boxed{\#E(\mathbb F_{q^n})=(1-\alpha^n)(1-q^n\alpha^{-n}),
\qquad |\alpha|=\sqrt q\quad(n\ge1).}
$$

This is the [elliptic-curve point count over a finite field](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-point-count-over-a-finite-field) formula and the [Riemann hypothesis for an elliptic curve over a finite field](../../../normalization-of-an-algebraic-curve.md#riemann-hypothesis-for-an-elliptic-curve-over-a-finite-field). In particular the powers on both factors are necessary; they are damaged in the converted TeX but present in the original PDF.

## 2

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Put $F=x^3+y^3+13z^3-2xyz$. The [Hessian criterion for flexes of a plane cubic](../../../normalization-of-an-algebraic-curve.md#hessian-criterion-for-flexes-of-a-plane-cubic) applies because the projective cubic is smooth. To check smoothness, a singular point with all coordinates nonzero would satisfy $3x^2=2yz$, $3y^2=2xz$, $39z^2=2xy$. Multiplication would force $351=8$, a contradiction. If one coordinate is zero, the three equations force all coordinates to vanish, which is not a projective point.

For completeness, the [Hessian criterion for flexes of a plane cubic](../../../normalization-of-an-algebraic-curve.md#hessian-criterion-for-flexes-of-a-plane-cubic) follows locally by putting a smooth point at $(0:0:1)$ and its tangent at $y=0$. After normalization the homogeneous cubic has terms $yz^2+ax^2z+bxyz+cy^2z$ and terms cubic in $x,y$. Its tangent has contact order three precisely when $a=0$. Its [Hessian matrix](../../../calculus.md#hessian-matrix) at the point has determinant $-8a$, giving exactly the same condition.

For the present cubic the Hessian determinant is

$$
\det\begin{pmatrix}
6x&-2z&-2y\\
-2z&6y&-2x\\
-2y&-2x&78z
\end{pmatrix}
=-24(x^3+y^3+13z^3)+2792xyz.
$$

On $F=0$ this is $2744xyz=8\cdot343\,xyz$. Thus the [plane cubic flexes](../../../normalization-of-an-algebraic-curve.md#inflection-point-of-a-plane-cubic) are exactly the points on the cubic with $xyz=0$. Let $c=\sqrt[3]{13}$ and let $\omega$ be a primitive cube root of unity. The complete list over the [algebraic closure](../../../algebra.md#algebraic-closure) is

$$
\boxed{(1:-\omega^j:0),\quad(-c\omega^j:0:1),\quad(0:-c\omega^j:1),\qquad j=0,1,2.}
$$

These nine points are distinct, and the Hessian calculation proves there are no others. They are the [flexes of a Hesse cubic](../../../normalization-of-an-algebraic-curve.md#flexes-of-a-hesse-cubic). The only rational one is $O'=(1:-1:0)$: the other two points with $z=0$ require a nonrational cube root of unity, and a rational point in either remaining triple would give a rational cube root of $-13$. By prime valuations, $13$ is not a rational cube.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For this [Weierstrass equation of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve), the inverse is $(x,y)\mapsto(x,13-y)$. At a point with $2y-13\ne0$, implicit differentiation gives the tangent slope

$$
m=\frac{3x^2+2x+13}{2y-13}.
$$

If the tangent line is $y=mx+b$, substitution into the equation shows that the three intersection abscissae sum to $m^2-1$. Two of them equal the tangency abscissa $x$, so the third is $x_3=m^2-1-2x$. Reflecting the third intersection by the inverse formula gives the [elliptic curve group law from Riemann-Roch](../../../normalization-of-an-algebraic-curve.md#elliptic-curve-group-law-from-riemann-roch) doubling formula

$$
x(2R)=m^2-1-2x(R),\qquad
 y(2R)=13-y(R)+m\bigl(x(R)-x(2R)\bigr).
$$

For $P$, the slope is $13/(-13)=-1$, giving $x(2P)=0$ and $y(2P)=13$. For $Q$, the slope is $(12-4+13)/(6-13)=-3$, giving $x(2Q)=9-1+4=12$ and $y(2Q)=13-3+(-3)(-2-12)=52$. Hence

$$
\boxed{2P=(0,13)=-P,\qquad 2Q=(12,52).}
$$

In particular $P$ has order exactly three: it is nonidentity and $2P=-P$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

We bound the [torsion subgroups](../../../group-theory.md#torsion-subgroup) by [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve). At a prime $p$ of [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve), reduction is injective on the prime-to-$p$ torsion. Indeed, a point in the kernel is represented by the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve) on the maximal ideal. Multiplication by an integer prime to $p$ has a unit linear coefficient and is invertible there, so the kernel has no nonzero torsion of such order.

Both curves have [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) at $2$ and $5$. For $E$ this follows from $\Delta=-91^3$, which is a unit at both primes. For $E'$ at $2$, its reduction is $x^3+y^3+z^3=0$ and its three partial derivatives cannot vanish at a projective point. At $5$, the singularity calculation in part (i) would require $351-8=343$ to vanish modulo $5$, which it does not; $3$ and $13$ are also units there.

Direct counting gives:

| Curve | Affine over $\mathbb F_2$ | At infinity | Total | Affine over $\mathbb F_5$ | At infinity | Total |
| --- | --- | --- | --- | --- | --- | --- |
| $E$ | $2$ | $1$ | $3$ | $8$ | $1$ | $9$ |
| $E'$ | $2$ | $1$ | $3$ | $8$ | $1$ | $9$ |

For $E$ over $\mathbb F_5$, the numbers of ordinate solutions at $x=0,1,2,3,4$ are $2,2,2,2,0$. For $E'$ in the chart $z=1$, they are $1,2,0,3,2$, with the single infinity point $(1:-1:0)$. These give the displayed totals without identifying the finite-field groups through the given [isogeny of elliptic curves](../../../normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves).

For either rational [torsion subgroup](../../../group-theory.md#torsion-subgroup), every odd-primary part injects at $2$, so the whole odd torsion has order dividing three. The two-primary part injects at $5$ and must be trivial, since the reduced group has odd order nine. Thus either rational [torsion subgroup](../../../group-theory.md#torsion-subgroup) has order at most three. For $E$, the point $P$ already has order three, so

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\{O,(0,0),(0,13)\}\cong\mathbb Z/3\mathbb Z.}
$$

For the plane cubic $E'$, the chosen identity $O'$ is a [plane cubic flex](../../../normalization-of-an-algebraic-curve.md#inflection-point-of-a-plane-cubic). The fact that [three-torsion points are flexes of a plane cubic](../../../normalization-of-an-algebraic-curve.md#three-torsion-points-are-flexes-of-a-plane-cubic) therefore identifies $E'[3]$ with its nine geometric flexes. Part (i) found only the identity among the rational flexes. No nonidentity rational three-torsion exists, and the preceding bound excludes every other order. Hence

$$
\boxed{E'(\mathbb Q)_{\mathrm{tors}}=\{O'\}.}
$$

This also illustrates that [isogenous elliptic curves can have different rational point groups](../../../normalization-of-an-algebraic-curve.md#isogenous-elliptic-curves-can-have-different-rational-point-groups); the given degree-three isogeny does not imply equality of rational torsion.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Double $2Q=(12,52)$ using the tangent formula. The slope is

$$
m=\frac{3\cdot12^2+2\cdot12+13}{2\cdot52-13}=\frac{469}{91}=\frac{67}{13},
$$

so

$$
4Q=\left(\frac{264}{169},\frac{32505}{2197}\right).
$$

This finite point is neither $P$ nor $-P$, since its abscissa is nonzero. Therefore $P\pm4Q$ are both finite nonidentity points.

For a direct exact-coordinate proof, the line from $P$ to $4Q$ has slope $985/104$, while the line from $P$ to $-4Q=(264/169,-3944/2197)$ has slope $-493/429$. For a secant through $P=(0,0)$ and $R=(u,v)$, its slope is $m=v/u$, and the group law gives $x(P+R)=m^2-1-u$, $y(P+R)=13-mx(P+R)$. Simplification yields

$$
\boxed{P+4Q=\left(\frac{5577}{64},-\frac{415909}{512}\right),\qquad
P-4Q=\left(-\frac{1352}{1089},\frac{415909}{35937}\right).}
$$

The first abscissa has odd numerator and denominator $64$. The second has denominator $1089=3^2\cdot11^2$ and numerator not divisible by either $3$ or $11$. Thus **neither point has integral coordinates**.

Reduction also explains the obstruction without requiring the full secant arithmetic. At the good prime $2$, $\overline Q=(0,1)=-\overline P$, and $\overline P$ has order three, so $\overline{P+4Q}=O$. At the good prime $11$, the displayed coordinates of $4Q$ reduce to $(0,0)=\overline P$, so $\overline{P-4Q}=O$. A finite point with integral affine coordinates reduces to an affine point, not to the identity at infinity. Membership in the [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve) therefore certifies the same two nonintegrality conclusions, at primes $2$ and $11$ respectively.

## 3

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

A one-dimensional commutative [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law) over the [p-adic integers](../../../number-theory.md#p-adic-integer) is a power series $\mathcal F(X,Y)\in\mathbb Z_p[[X,Y]]$ with

$$
\mathcal F(X,0)=X,\quad \mathcal F(0,Y)=Y,\quad
\mathcal F(X,Y)=\mathcal F(Y,X),
$$



$$
\mathcal F(\mathcal F(X,Y),Z)=\mathcal F(X,\mathcal F(Y,Z)).
$$

Its linear part is $X+Y$, and it has a unique [formal inverse](../../../normalization-of-an-algebraic-curve.md#formal-inverse) $i(T)=-T+O(T^2)$ satisfying $\mathcal F(T,i(T))=0$. A formal-group homomorphism is a series $h(T)\in T\mathbb Z_p[[T]]$ satisfying $h(\mathcal F(X,Y))=\mathcal F(h(X),h(Y))$.

Define $[n](T)$ by adding $T$ to itself $n$ times with the [formal group law](../../../normalization-of-an-algebraic-curve.md#formal-group-law). Induction on the linear part gives

$$
[n](T)=nT+O(T^2).
$$

Associativity and commutativity make $[n]$ a formal-group homomorphism. Since $p\nmid n$, its linear coefficient is a unit in $\mathbb Z_p$. We now construct its [compositional inverse of a formal power series](../../../commutative-algebra.md#compositional-inverse-of-a-formal-power-series), rather than merely assert that the nonzero coefficient is sufficient.

Write $[n](T)=nT+a_2T^2+\cdots$ and seek $g(T)=b_1T+b_2T^2+\cdots$ with $[n](g(T))=T$. The degree-one coefficient gives $b_1=n^{-1}$. At degree $k\ge2$, the coefficient is $nb_k$ plus a polynomial in the already chosen $b_1,\ldots,b_{k-1}$ and $a_2,\ldots,a_k$. Division by the unit $n$ uniquely chooses $b_k\in\mathbb Z_p$. This recursively constructs $g$ over the same ring. A right inverse is constructed in the same way; associativity of composition identifies it with $g$, so $g\circ[n]=[n]\circ g=T$.

To prove that $g$ respects the group law, apply $[n]$ to the two candidate series:

$$
[n]\bigl(\mathcal F(g(X),g(Y))\bigr)
=\mathcal F(X,Y)
=[n]\bigl(g(\mathcal F(X,Y))\bigr).
$$

Cancel by composing with $g$. The result is $\mathcal F(g(X),g(Y))=g(\mathcal F(X,Y))$. Thus

$$
\boxed{[n]:\mathcal F\longrightarrow\mathcal F\text{ is an isomorphism over }\mathbb Z_p.}
$$

This is the [multiplication isomorphism of a formal group law](../../../normalization-of-an-algebraic-curve.md#multiplication-isomorphism-of-a-formal-group-law), a special case of the [invertible morphism criterion for formal group laws](../../../normalization-of-an-algebraic-curve.md#invertible-morphism-criterion-for-formal-group-laws). If $p\mid n$, its linear coefficient is not a unit, so the same isomorphism assertion would fail.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Reduce $P$ to $\overline P\in\widetilde E(\mathbb F_p)$. Because $p\nmid n$, the [multiplication-by-n morphism](../../../ringed-space.md#multiplication-by-n-morphism) on the reduced [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) is a separable, surjective morphism of degree $n^2$. Choose a point $\overline Q\in\widetilde E(\overline{\mathbb F}_p)$ with $n\overline Q=\overline P$. Its coordinates lie in some finite field $\mathbb F_{p^d}$.

Let $L/\mathbb Q_p$ be the finite [unramified extension](../../../arithmetic.md#unramified-extension) with residue field $\mathbb F_{p^d}$. The curve retains [good reduction](../../../normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) over $L$. Its smooth integral model and the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) give [surjectivity of good reduction over a local field](../../../normalization-of-an-algebraic-curve.md#surjectivity-of-good-reduction-over-a-local-field), so lift $\overline Q$ to some $Q_0\in E(L)$. This lift need not satisfy $nQ_0=P$ exactly, but its error

$$
R=P-nQ_0
$$

has zero reduction and belongs to $E_1(L)$, the [kernel of reduction of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve).

The parameter $t=-x/y$ at infinity identifies $E_1(L)$ with the maximal ideal $\mathfrak m_L$ equipped with the [formal group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve). The integral power series for $[n]$ and its inverse from part (i) remain integral over $\mathcal O_L$. They converge on $\mathfrak m_L$: terms of degree $k$ tend to zero in valuation because their coefficients are integral and the argument has positive valuation. Hence multiplication by $n$ is bijective on $E_1(L)$. Choose its unique solution $T\in E_1(L)$ to $nT=R$, and put $Q=Q_0+T$. Then

$$
\boxed{Q\in E(L),\qquad nQ=nQ_0+R=P,\qquad L/\mathbb Q_p\text{ finite unramified}.}
$$

The residue-field extension supplies a division point modulo $p$, and the formal-group inverse corrects the error without introducing ramification. This is the local construction underlying the [uniform unramified division field over a local field](../../../normalization-of-an-algebraic-curve.md#uniform-unramified-division-field-over-a-local-field) and [unramified division torsors at good primes](../../../normalization-of-an-algebraic-curve.md#unramified-division-torsors-at-good-primes).

## 4

↑ **Parent:** [Paper 28](paper-28.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [congruent number](../../../normalization-of-an-algebraic-curve.md#congruent-number) is a positive integer which occurs as the area of a [right triangle](../../../geometry-and-topology.md#right-triangle) with positive rational side lengths. Scaling a triangle by a nonzero rational factor multiplies its area by a rational square, so the essential parameter is its positive square class; integer parameters can be reduced to [square-free integers](../../../number-theory.md#square-free-integer). For example $6$ is congruent by the triangle $(3,4,5)$, and $5$ is congruent by $(3/2,20/3,41/6)$.

The connection with [elliptic curves](../../../normalization-of-an-algebraic-curve.md#elliptic-curve) comes from the [congruent number elliptic curve](../../../normalization-of-an-algebraic-curve.md#congruent-number-elliptic-curve) in the model

$$
E_N:\quad y^2=x^3-N^2x.
$$

From a rational point with $y\ne0$, define

$$
a=\left|\frac{x^2-N^2}{y}\right|,\qquad
b=\left|\frac{2Nx}{y}\right|,\qquad
c=\left|\frac{x^2+N^2}{y}\right|.
$$

Direct squaring gives $a^2+b^2=c^2$, and its area is

$$
\frac{ab}{2}=\frac{N|x(x^2-N^2)|}{y^2}=N.
$$

Conversely, from a positive rational triangle $(a,b,c)$ of area $N$, put

$$
x=N\frac{c+a}{b},\qquad y=2N^2\frac{c+a}{b^2}.
$$

Substitution using $c^2=a^2+b^2$ and $ab=2N$ gives $y^2=x^3-N^2x$ and $y\ne0$. Thus

$$
\boxed{N\text{ congruent}\iff E_N(\mathbb Q)\text{ has a point with }y\ne0.}
$$

The standard [rational torsion of a congruent number curve](../../../normalization-of-an-algebraic-curve.md#rational-torsion-of-a-congruent-number-curve) consists of $O,(0,0),(N,0),(-N,0)$. One way to see the torsion restriction is to use good primes $p\equiv3\pmod4$. The character sum cancels at $x$ and $-x$, giving $\#E_N(\mathbb F_p)=p+1$. For any odd prime $\ell$, the [Dirichlet theorem on primes in arithmetic progressions](../../../analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions) supplies good primes with $p\equiv3\pmod4$ and $p\equiv1\pmod\ell$, so the [reduction of torsion points on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve) excludes $\ell$-torsion. Good primes $p\equiv3\pmod8$ similarly bound the two-primary torsion by four, and the four displayed points give equality. Consequently the [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group) turns the criterion into **positive rank of $E_N(\mathbb Q)$**. Arithmetic [two-descent on an elliptic curve](../../../normalization-of-an-algebraic-curve.md#two-descent-on-an-elliptic-curve) and local obstructions are therefore tools for the congruent number problem, and a nontorsion point gives [infinitely many rational right triangles from a nontorsion point](../../../normalization-of-an-algebraic-curve.md#infinitely-many-rational-right-triangles-from-a-nontorsion-point) by taking multiples.

We now give elementary proofs for $1$ and $2$, including the descent steps. Recall the [primitive Pythagorean parametrization](../../../geometry-and-topology.md#primitive-pythagorean-parametrization)

$$
A=2mn,\qquad B=m^2-n^2,\qquad C=m^2+n^2,
$$

where $m>n>0$ are coprime and of opposite parity. To derive it, in a primitive [Pythagorean triple](../../../geometry-and-topology.md#pythagorean-triple) put the even leg at $A$. The relatively prime integers $(C+B)/2,(C-B)/2$ have product $(A/2)^2$, so each is a square, say $m^2,n^2$. This gives the formulas and the parity condition. The area is $mn(m-n)(m+n)$, and its four factors are pairwise coprime: their common divisors reduce to divisors of $m,n$ or of two, while $m\pm n$ are odd.

**Area one is impossible.** Clearing denominators of a hypothetical rational triangle of area one gives an integer triangle with square area. Dividing out its common factor leaves a primitive integer triangle whose area is still a rational square; an integer which is a rational square is an integer square. Choose such a triangle with smallest hypotenuse. Pairwise coprimality in the area product forces

$$
m=r^2,\qquad n=s^2,\qquad m+n=u^2,\qquad m-n=v^2.
$$

The positive integers $u,v$ are odd and coprime. If $m$ were even, then $n$ would be odd and $u^2-v^2=2s^2$ would be $2$ modulo eight, whereas two odd squares have difference zero modulo eight. Hence $m$ is odd, $n$ is even and $s$ is even.

Now set $a=(u+v)/2$ and $b=(u-v)/2$. These are positive coprime integers and

$$
a^2+b^2=\frac{u^2+v^2}{2}=m=r^2,\qquad
\frac{ab}{2}=\frac{u^2-v^2}{8}=\frac{s^2}{4}.
$$

Thus $(a,b,r)$ is another integer [right triangle](../../../geometry-and-topology.md#right-triangle) with square area and hypotenuse $r$, strictly smaller than $m^2+n^2$. This contradicts the minimal choice and proves the [Fermat right triangle theorem](../../../normalization-of-an-algebraic-curve.md#fermat-right-triangle-theorem). In particular **$1$ is not a congruent number**.

For area two we first establish the auxiliary descent [fourth-power sum cannot be a square](../../../number-theory.md#fourth-power-sum-cannot-be-a-square). Suppose $x^4+y^4=z^2$ with positive integers, and choose a primitive solution with smallest $z$. Two odd fourth powers sum to $2$ modulo sixteen, so after exchange $x$ is odd and $y$ is even. Parametrize the primitive triangle $(x^2,y^2,z)$:

$$
x^2=m^2-n^2,\qquad y^2=2mn,\qquad z=m^2+n^2.
$$

The case $m$ even, $n$ odd makes $x^2\equiv3\pmod4$, so $m$ is odd and $n$ even. Coprimality then gives $m=u^2$ and $n=2v^2$. Consequently

$$
x^2+(2v^2)^2=(u^2)^2.
$$

This second triangle is primitive, since $x$ is odd and $\gcd(x,v)=1$. Parametrize it as $x=r^2-s^2$, $2v^2=2rs$, $u^2=r^2+s^2$, with $r,s$ coprime. The equality $v^2=rs$ makes $r=a^2$, $s=b^2$. Thus

$$
a^4+b^4=u^2,
$$

a new positive solution with smaller hypotenuse $u<z=u^4+4v^4$. This contradicts [infinite descent](../../../number-theory.md#infinite-descent), proving the auxiliary assertion.

**Area two is also impossible.** Clearing denominators and removing a common factor now gives a primitive integer triangle with area twice an integer square. Indeed, if an integer is $2(a/b)^2$ with $\gcd(a,b)=1$, then $b^2$ divides two, forcing $b=1$. Its area product would satisfy

$$
mn(m-n)(m+n)=2t^2.
$$

The odd factors must be squares and the unique even factor twice a square. As in the preceding modulo-eight argument, $m$ even would force $m+n=c^2$, $m-n=d^2$ and $n=b^2$ odd, with $c^2-d^2=2b^2$, impossible modulo eight. Thus

$$
m=a^2,\qquad n=2b^2,\qquad m+n=c^2,\qquad m-n=d^2.
$$

The integers $u=(c+d)/2$ and $v=(c-d)/2$ are positive and coprime, and $uv=(c^2-d^2)/4=b^2$. Hence $u=r^2$, $v=s^2$. But

$$
a^2=m=\frac{c^2+d^2}{2}=u^2+v^2=r^4+s^4,
$$

contradicting the auxiliary descent. This proves [two is not a congruent number](../../../normalization-of-an-algebraic-curve.md#two-is-not-a-congruent-number), and concludes

$$
\boxed{1\text{ and }2\text{ are not congruent numbers}.}
$$

The two obstructions are global arithmetic descents. The elliptic-curve correspondence organizes the wider problem, but by itself is not a substitute for proving these particular nonexistence assertions.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $K$ be a field, $K_s$ a separable closure and $G_K$ its [absolute Galois group](../../../galois-theory.md#absolute-galois-group). A discrete [Galois module](../../../galois-theory.md#galois-module) $A$ is an abelian group with a continuous $G_K$-action, so each element has an open stabilizer. [Galois cohomology](../../../galois-theory.md#galois-cohomology) uses continuous cochains. Its zeroth group is $H^0(K,A)=A^{G_K}$, and its first group is

$$
H^1(K,A)=Z^1(K,A)/B^1(K,A),
$$

where

$$
c_{\sigma\tau}=c_\sigma+\sigma c_\tau,
\qquad
B^1(K,A)=\{c_\sigma=\sigma a-a:a\in A\}.
$$

Thus cocycles measure a failure of descent, and coboundaries account for changing a chosen lift. A short exact sequence of [Galois modules](../../../galois-theory.md#galois-module) gives a [long exact sequence in group cohomology](../../../group-theory.md#long-exact-sequence-in-group-cohomology). Its connecting map sends an invariant element of a quotient to the cocycle $\sigma b-b$ of a chosen lift $b$; changing the lift changes this by a coboundary. These constructions provide the bridge between arithmetic divisibility and cohomology.

For [Kummer theory](../../../galois-theory.md#kummer-theory), assume the characteristic does not divide $n$. The multiplicative exact sequence is

$$
1\longrightarrow\mu_n\longrightarrow K_s^\times
\xrightarrow{,n,}K_s^\times\longrightarrow1.
$$

The final arrow is surjective because a root of $T^n-a$ is separable for $a\ne0$. [Hilbert's theorem 90](../../../galois-theory.md#hilbert-s-theorem-90) says $H^1(K,K_s^\times)=0$. Here is its usual finite-extension proof. For a multiplicative cocycle $c_\sigma$ on a finite [Galois extension](../../../galois-theory.md#finite-galois-extension) $L/K$, choose $a\in L$ so that

$$
A=\sum_{\sigma\in\operatorname{Gal}(L/K)}c_\sigma\sigma(a)\ne0.
$$

Such an $a$ exists by the [Artin independence theorem](../../../galois-theory.md#linear-independence-of-distinct-field-embeddings). The cocycle identity gives $\tau A=c_\tau^{-1}A$. With $b=A^{-1}$ this becomes $c_\tau=\tau b/b$, a coboundary. Every continuous cocycle with values in $K_s^\times$ is defined over a sufficiently large finite Galois extension, so the same result holds for the absolute group.

The [long exact sequence in group cohomology](../../../group-theory.md#long-exact-sequence-in-group-cohomology) now gives

$$
\boxed{H^1(K,\mu_n)\cong K^\times/(K^\times)^n.}
$$

The class of $a$ maps to $c_\sigma=\sigma(\alpha)/\alpha$, where $\alpha^n=a$. This cohomological statement does not require $\mu_n\subset K$; it retains the actual Galois action on $\mu_n$. If all $n$th roots of unity do lie in $K$, the action is trivial, and after choosing a primitive root of unity the cocycles are characters into $\mathbb Z/n\mathbb Z$. Thus adjoining an $n$th root of $a$ describes a cyclic extension of degree dividing $n$, and Kummer classes classify the corresponding characters. For $n=2$, this gives the familiar quadratic extensions and the [square-class group of a field](../../../galois-theory.md#square-class-group-of-a-field).

Now let $K$ be a [number field](../../../algebraic-number-theory.md#number-field) and $E/K$ an [elliptic curve](../../../normalization-of-an-algebraic-curve.md#elliptic-curve). The [multiplication-by-n morphism](../../../ringed-space.md#multiplication-by-n-morphism) is a surjective isogeny on $E(\overline K)$, with kernel $E[n]\cong(\mathbb Z/n\mathbb Z)^2$. The [Kummer exact sequence of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-exact-sequence-of-an-elliptic-curve)

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)
\xrightarrow{[n]}E(\overline K)\longrightarrow0
$$

yields

$$
0\longrightarrow E(K)/nE(K)\xrightarrow{\delta}
H^1(K,E[n])\longrightarrow H^1(K,E)[n]\longrightarrow0.
$$

Explicitly, choose $Q$ with $nQ=P$ and set $\delta(P)_\sigma=\sigma Q-Q$. This lies in $E[n]$, satisfies the cocycle identity and is unchanged as a class if $Q$ is replaced by another division point. If it is a coboundary $\sigma T-T$ for $T\in E[n]$, then $Q-T$ is rational over $K$ and $P=n(Q-T)$. Conversely such a rational division point makes the cocycle zero. This proves the injectivity of the [Kummer map of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve) on $E(K)/nE(K)$.

To prove the [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem), it remains to prove that this particular cohomological image is finite. The full group $H^1(K,E[n])$ need not be finite, so the injection alone is not enough. Choose a finite set $S$ of finite places containing the bad-reduction places and those dividing $n$. At any other place, the construction in Question 3 works over the local field: reduce $P$, find an $n$-division point over a finite residue extension, lift it by the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma), and correct its error by the inverse formal multiplication. Thus $P$ has an $n$-division point over the [maximal unramified extension](../../../arithmetic.md#maximal-unramified-extension). Choosing that lift locally makes the cocycle zero on inertia. For an arbitrary lift its restriction is a coboundary, so the cohomology class is unramified. Therefore the image lies in [first Galois cohomology unramified outside a finite set](../../../galois-theory.md#first-galois-cohomology-unramified-outside-a-finite-set):

$$
\delta(E(K)/nE(K))\subseteq H^1_S(K,E[n]).
$$

We prove the required finiteness of this group. Take a finite Galois extension $L/K$ containing all of $E[n]$ and $\mu_n$, and enlarge $S$ to include any remaining ramification of $L/K$. Let $S_L$ be the places above it. The [inflation-restriction exact sequence](../../../group-theory.md#inflation-restriction-exact-sequence) bounds the kernel of restriction to $L$ by

$$
H^1(\operatorname{Gal}(L/K),E[n]),
$$

a finite group, since both its group of arguments and its group of values are finite. Over $L$ the torsion module is constant and can be identified with $\mu_n^2$, so [Kummer theory](../../../galois-theory.md#kummer-theory) gives

$$
H^1(L,E[n])\cong\bigl(L^\times/(L^\times)^n\bigr)^2.
$$

Restrictions of our unramified classes remain unramified outside $S_L$. If a Kummer class $[a]$ is unramified at such a place $v$, its $n$th root can be taken in an unramified local extension. The extended valuation still has integer values, and $n\,v(\sqrt[n]a)=v(a)$. Hence $v(a)$ is divisible by $n$. Each coordinate therefore lies in the [S-unramified power class group](../../../normalization-of-an-algebraic-curve.md#s-unramified-power-class-group)

$$
L(S_L,n)=\{[a]\in L^\times/(L^\times)^n:
 v(a)\equiv0\pmod n\text{ for }v\notin S_L\}.
$$

This group is finite. Indeed, the ideal of $a$ away from $S_L$ is $\mathfrak a^n$. Sending $[a]$ to $[\mathfrak a]$ yields the exact sequence

$$
0\longrightarrow\mathcal O_{L,S_L}^{\times}/(\mathcal O_{L,S_L}^{\times})^n
\longrightarrow L(S_L,n)
\longrightarrow\operatorname{Cl}(\mathcal O_{L,S_L})[n]\longrightarrow0.
$$

For its kernel, a principal $\mathfrak a$ lets us divide $a$ by an $n$th power to obtain an $S_L$-unit. For surjectivity, an ideal class killed by $n$ has an $n$th power which is principal away from $S_L$, giving such an $a$. The [S-unit group](../../../algebra.md#s-unit-group) is finitely generated and the [ideal class group](../../../algebraic-number-theory.md#ideal-class-group) is finite; hence both end groups are finite, proving [finiteness of S-unramified Kummer classes](../../../normalization-of-an-algebraic-curve.md#finiteness-of-s-unramified-kummer-classes). Restriction has finite image in $L(S_L,n)^2$ and finite kernel, so $H^1_S(K,E[n])$ is finite. We conclude

$$
\boxed{\#\bigl(E(K)/nE(K)\bigr)<\infty\qquad(n\ge2),}
$$

which is the [Weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem) and its [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#kummer-theoretic-proof-of-the-weak-mordell-weil-theorem).

This framework also defines the [Selmer group of an elliptic curve](../../../normalization-of-an-algebraic-curve.md#n-selmer-group) by imposing that a class in $H^1(K,E[n])$ lie in the local Kummer image at every completion. Its classes are unramified outside a fixed finite set, so the same finiteness proof applies. Its relation to rational points is

$$
0\longrightarrow E(K)/nE(K)\longrightarrow
\operatorname{Sel}^{(n)}(E/K)\longrightarrow
\operatorname{Sha}(E/K)[n]\longrightarrow0.
$$

The [Tate–Shafarevich group](../../../normalization-of-an-algebraic-curve.md#tate-shafarevich-group) here measures the difference between locally soluble torsors and globally soluble ones. Finally, the weak theorem gives finite divisibility quotients; adding the [height descent lemma](../../../normalization-of-an-algebraic-curve.md#height-descent-lemma) and bounded-height finiteness proves the stronger [Mordell-Weil theorem](../../../normalization-of-an-algebraic-curve.md#mordell-weil-group). Those height inputs are additional to the cohomological finiteness just established.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
