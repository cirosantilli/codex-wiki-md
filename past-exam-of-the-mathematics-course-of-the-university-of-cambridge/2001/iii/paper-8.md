# Paper 8

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper8.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper8.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use [polar coordinates](../../../calculus.md#polar-coordinates) $x=r\cos\theta$, $y=r\sin\theta$. Away from the crossing, the [lemniscate of Bernoulli](../../../algebraic-geometry.md#lemniscate-of-bernoulli) has $r^2=\cos2\theta$. An explicit parametrization of its four quarter-arcs is

$$
\boxed{x=\pm t\sqrt{\frac{1+t^2}{2}},\qquad y=\pm t\sqrt{\frac{1-t^2}{2}},\qquad 0\leq t\leq1},
$$

where the two signs are independent. Indeed $x^2+y^2=t^2$ and $x^2-y^2=t^4$. The four arcs meet at the origin and at the two lobe endpoints, covering the entire curve.

For the upper-right quarter, take $0\leq\theta\leq\pi/4$, $r=\sqrt{\cos2\theta}$. Differentiating gives $dr/d\theta=-\sin2\theta/r$. Thus the [arc length](../../../riemannian-geometry.md#arc-length) element satisfies

$$
\left(\frac{ds}{d\theta}\right)^2=r^2+\left(\frac{dr}{d\theta}\right)^2
=\frac{\cos^22\theta+\sin^22\theta}{\cos2\theta}=\frac1{r^2}.
$$

Set $t=r$, which decreases from one to zero. Since $|dt/d\theta|=\sqrt{1-t^4}/t$, it follows that $ds=|dt|/\sqrt{1-t^4}$. All four quarter-arcs have the same length, so

$$
\boxed{L=4\int_0^1\frac{dt}{\sqrt{1-t^4}}}.
$$

The endpoint singularity is proportional to $(1-t)^{-1/2}$ and is integrable. This is the geometric origin of the [lemniscatic integral](../../../complex-analysis.md#lemniscatic-integral).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Choose the [holomorphic square root](../../../complex-analysis.md#holomorphic-square-root) in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) whose boundary value is positive on $0<x<1$. Its primitive has [derivative](../../../calculus.md#derivative) $F_1'(z)=1/\sqrt{z(1-z^2)}$. The integral from the boundary basepoint zero is well-defined by a limiting path: the local singularity is only $z^{-1/2}$.

The three finite [prevertices](../../../geometry-and-topology.md#prevertex-of-a-schwarz-christoffel-map) $-1,0,1$ have [derivative](../../../calculus.md#derivative) exponent $-1/2$, hence image angle $\pi/2$. At infinity $F_1'(z)=O(z^{-3/2})$, so the local coordinate $1/z$ also gives image angle $\pi/2$. These are the four corners of a [Schwarz-Christoffel mapping](../../../geometry-and-topology.md#schwarz-christoffel-mapping) to a [rectangle](../../../geometry-and-topology.md#rectangle). To establish that it is a [square](../../../geometry-and-topology.md#square) rather than a general [rectangle](../../../geometry-and-topology.md#rectangle), put

$$
A=\int_0^1\frac{dx}{\sqrt{x(1-x^2)}}.
$$

The length along $(-1,0)$ is also $A$ by $x\mapsto-x$. The length along $(1,\infty)$ is

$$
\int_1^\infty\frac{dx}{\sqrt{x(x^2-1)}}=A,
$$

by $x=1/t$, and the fourth side has the same length by [symmetry](../../../physics.md#symmetry-physics). With the chosen branch, the boundary [derivatives](../../../calculus.md#derivative) on the intervals $(-\infty,-1),(-1,0),(0,1),(1,\infty)$ have phases $-1,-i,1,i$, respectively. Therefore

$$
F_1(-1)=iA,\quad F_1(0)=0,\quad F_1(1)=A,\quad F_1(\infty)=A+iA.
$$

The extended real boundary maps continuously and once around this [square](../../../geometry-and-topology.md#square). Each side is traversed monotonically, and the four corner limits are finite. The [argument principle](../../../complex-analysis.md#argument-principle), applied after small indentations around the boundary singularities, counts one inverse image of each interior value and zero of each exterior value. Since $F_1'$ never vanishes in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), those interior inverse images are simple. Thus

$$
\boxed{F_1:\mathbb H\longrightarrow\{u+iv:0<u<A,\ 0<v<A\}\text{ is conformal and bijective}.}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Let $h(\zeta)=i(1+\zeta)/(1-\zeta)$, the inverse [Cayley transform between the half-plane and disk](../../../complex-analysis.md#cayley-transform-between-the-half-plane-and-disk). Direct calculation gives

$$
h'\!(\zeta)=\frac{2i}{(1-\zeta)^2},\qquad
h(\zeta)(1-h(\zeta)^2)=\frac{2i(1+\zeta)(1+\zeta^2)}{(1-\zeta)^3},
$$

so

$$
\left((F_1\circ h)'(\zeta)\right)^2=\frac{2i}{1-\zeta^4}.
$$

On the [unit disc](../../../topology.md#unit-disc), choose the [holomorphic square root](../../../complex-analysis.md#holomorphic-square-root) of $1-\zeta^4$ equal to one at zero. Both sides define nonvanishing [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) [derivatives](../../../calculus.md#derivative), and their quotient has constant square. The branch chosen in part ii gives $(F_1\circ h)'(0)=1+i$. Consequently

$$
F_1(h(\zeta))=F_1(i)+(1+i)F(\zeta).
$$

An affine change of image coordinate preserves [conformality](../../../geometry-and-topology.md#conformality), so the [lemniscatic integral](../../../complex-analysis.md#lemniscatic-integral) maps the disc bijectively onto a [square](../../../geometry-and-topology.md#square).

The normalization specifies the [square](../../../geometry-and-topology.md#square) exactly. Put $B=F(1)=\int_0^1dt/\sqrt{1-t^4}$. The substitution $x=t^2$ gives $A=2B$. The integral satisfies $F(-z)=-F(z)$ and $F(iz)=iF(z)$, so its four corner values are $B,iB,-B,-iB$. Thus

$$
\boxed{F(\mathbb D)=\{u+iv:|u|+|v|<B\}}.
$$

In particular the image is a [square](../../../geometry-and-topology.md#square) rotated through $\pi/4$ relative to the one in part ii, and its side length is $\sqrt2B$. These symmetries also give $F_1(i)=(1+i)B$ from the affine identity.

<a id="1/iii/image-the-lemniscate-and-the-four-corner-boundary-correspondence-of-the-lemniscatic-disc-to-square-map"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8-lemniscate-square.png)

**[Figure 1](#1/iii/image-the-lemniscate-and-the-four-corner-boundary-correspondence-of-the-lemniscatic-disc-to-square-map). The lemniscate and the four-corner boundary correspondence of the lemniscatic disc-to-square map**.

## 2

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For genuine degrees three and two, the [resultant](../../../polynomial.md#resultant) is the [Sylvester matrix](../../../polynomial.md#sylvester-matrix) [determinant](../../../linear-algebra.md#determinant)

$$
\boxed{R(p,q)=\det\begin{pmatrix}
a&b&c&d&0\\0&a&b&c&d\\
\alpha&\beta&\gamma&0&0\\0&\alpha&\beta&\gamma&0\\0&0&\alpha&\beta&\gamma
\end{pmatrix}}.
$$

Equivalently, if $r_1,r_2,r_3$ are the roots of $p$, counted with multiplicity, then $R(p,q)=a^2\prod_iq(r_i)$. Thus **$R(p,q)\ne0$ means that the [polynomials](../../../polynomial.md) have no common root**, or equivalently are coprime over $\mathbb C$. One can also see this from the matrix: its singularity gives a nonzero relation $Ap+Bq=0$ with $\deg A<2$, $\deg B<3$. If $p,q$ were coprime, $p\mid B$ would force $B=0$, then $A=0$, a contradiction. Conversely, a common factor supplies such a relation after dividing $p,q$ by that factor. When a leading coefficient is zero, use the [resultant](../../../polynomial.md#resultant) for the actual [polynomial](../../../polynomial.md) degrees rather than assuming the displayed fixed-degree criterion unchanged.

An [algebraic addition theorem](../../../isolated-singularity.md#algebraic-addition-theorem) for a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) $f$ means a nonzero [polynomial](../../../polynomial.md) $P(U,V,W)$ with

$$
P(f(z),f(w),f(z+w))=0
$$

identically where the values are finite. A local relation extends meromorphically to the other regular arguments.

For a [polynomial](../../../polynomial.md) $f$ of positive degree $d$, let $z_i$ be the $d$ roots of $f(z)-U$ and $w_j$ the $d$ roots of $f(w)-V$. Form

$$
P(U,V,W)=\prod_{i=1}^d\prod_{j=1}^d\bigl(W-f(z_i+w_j)\bigr).
$$

Its coefficients are separately [symmetric polynomials](../../../polynomial.md#symmetric-polynomial) in the two sets of roots. The [Fundamental theorem of symmetric polynomials](../../../polynomial.md#fundamental-theorem-of-symmetric-polynomials) and the fixed nonzero leading coefficient of $f$ show they are [polynomials](../../../polynomial.md) in $U,V$. The expression is monic of degree $d^2$ in $W$, so it is nonzero. If $U=f(z)$, $V=f(w)$, one factor vanishes at $W=f(z+w)$. This proves the addition relation, including at exceptional multiple-root values by [polynomial](../../../polynomial.md) identity. A constant [polynomial](../../../polynomial.md) instead has the relation $W-f(0)=0$.

For the elliptic case, let $E=\mathbb C/\Lambda$. A nonconstant [elliptic function](../../../complex-analysis.md#elliptic-function) $f$ defines a [finite morphism](../../../algebraic-geometry.md#finite-morphism) $E\to\mathbb P^1$, so the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) of $E$ is a finite [algebraic extension](../../../algebra.md#algebraic-extension) of $\mathbb C(f)$. The [elliptic function-field decomposition](../../../complex-analysis.md#elliptic-function-field-decomposition) expresses it as $\mathbb C(\wp,\wp')$, with

$$
(\wp')^2=4\wp^3-g_2\wp-g_3.
$$

The [Weierstrass addition formula](../../../complex-analysis.md#weierstrass-addition-formula) makes translation algebraic:

$$
\wp(z+w)=-\wp(z)-\wp(w)+\frac14\left(\frac{\wp'(z)-\wp'(w)}{\wp(z)-\wp(w)}\right)^2.
$$

Differentiating and using the cubic differential equation also makes $\wp'(z+w)$ rational in the four separate values. Therefore $f(z+w)$ lies in a finite [algebraic extension](../../../algebra.md#algebraic-extension) of $\mathbb C(f(z),f(w))$. Its algebraic equation, after clearing denominators, is the required [polynomial](../../../polynomial.md) relation. This sketches why every [elliptic function](../../../complex-analysis.md#elliptic-function), not only $\wp$, has an [algebraic addition theorem](../../../isolated-singularity.md#algebraic-addition-theorem). Constants are already covered.

For the final assertion, consider $f(z)=e^{e^z}$, an [entire function](../../../complex-analysis.md#entire-function). If $c$ is a period, then $e^{e^z(e^c-1)}=1$ for every $z$. The continuous exponent must be a constant integer multiple of $2\pi i$; its [derivative](../../../calculus.md#derivative) forces $e^c=1$. Hence its periods are exactly $2\pi i\mathbb Z$, making it a [simply periodic function](../../../function.md#simply-periodic-function).

Suppose it had an [algebraic addition theorem](../../../isolated-singularity.md#algebraic-addition-theorem) $P$. There are only finitely many values $V_0$ for which $P(U,V_0,W)$ is identically zero: a nonzero coefficient [polynomial](../../../polynomial.md) in $V$ already bounds this exceptional set. Choose a positive irrational $\alpha$ with $e^\alpha$ outside this set, and set $c=\log\alpha$. Specializing $w=c$ gives a nonzero [polynomial](../../../polynomial.md) $Q(U,W)=P(U,e^\alpha,W)$ and, with $t=e^z$,

$$
0=Q(e^t,e^{\alpha t})=\sum_{m,n}q_{mn}e^{(m+\alpha n)t}.
$$

All exponents with nonzero coefficients are distinct, by irrationality of $\alpha$. Divide by the exponential with largest real exponent and let $t\to+\infty$; its nonzero coefficient would have to tend to zero. This contradiction proves that **simple periodicity does not imply an [algebraic addition theorem](../../../isolated-singularity.md#algebraic-addition-theorem)**. It is the [simply periodic entire function without an algebraic addition theorem](../../../isolated-singularity.md#simply-periodic-entire-function-without-an-algebraic-addition-theorem) example.

## 3

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take a real modulus $0<k<1$ and complementary modulus $k'=\sqrt{1-k^2}$. The [Jacobi elliptic sine](../../../complex-analysis.md#jacobi-elliptic-sine) is constructed by inverting a [Schwarz-Christoffel mapping](../../../geometry-and-topology.md#schwarz-christoffel-mapping). The main reason for the Schwarz-Christoffel [derivative](../../../calculus.md#derivative) is local angle behavior: if a [prevertex](../../../geometry-and-topology.md#prevertex-of-a-schwarz-christoffel-map) $a_j$ corresponds to a [polygon](../../../geometry-and-topology.md#polygon) angle $\pi\alpha_j$, straightening that corner gives $U(w)-U(a_j)\sim C_j(w-a_j)^{\alpha_j}$. Hence $U'$ has exponent $\alpha_j-1$. Along each straight boundary side its argument is constant. Dividing $U'$ by $\prod_j(w-a_j)^{\alpha_j-1}$ removes those angle changes; [Schwarz reflection](../../../complex-analysis.md#schwarz-reflection-principle) extends the quotient across the real boundary and the corner singularities. With all vertices finite, its behavior at infinity is also regular, because the sum of the [derivative](../../../calculus.md#derivative) exponents is $-2$. It is therefore a nonzero constant on the sphere. This yields

$$
U'(w)=C\prod_j(w-a_j)^{\alpha_j-1}.
$$

This argument explains the exponents, the branch choices and the role of boundary reflection, rather than just writing down the formula.

For a [rectangle](../../../geometry-and-topology.md#rectangle), four angles are $\pi/2$, so choose prevertices $-1/k,-1,1,1/k$ and normalize the inverse map as

$$
U(w)=\int_0^w\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}}.
$$

Use the branch positive on $(-1,1)$. Set

$$
K=\int_0^1\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}},\qquad K'=K(k').
$$

The two middle corner values are $U(\pm1)=\pm K$. The right side length is

$$
\int_1^{1/k}\frac{dt}{\sqrt{(t^2-1)(1-k^2t^2)}}=K',
$$

as the substitution $t=(1-k'^2s^2)^{-1/2}$ shows. The selected branch makes the increment along that side $iK'$. Thus the other corner values are $K+iK'$ and $-K+iK'$. The two boundary intervals through infinity have combined horizontal length $2K$; the substitution $t=1/(ks)$ gives length $K$ from $1/k$ to infinity. In particular $U(\infty)=iK'$. As in the [square](../../../geometry-and-topology.md#square) mapping, the boundary goes once around a [rectangle](../../../geometry-and-topology.md#rectangle), and the [argument principle](../../../complex-analysis.md#argument-principle) gives a [conformal](../../../geometry-and-topology.md#conformal-map) [bijection](../../../function.md#bijection)

$$
U:\mathbb H\longrightarrow\{-K<\operatorname{Re}z<K,\quad0<\operatorname{Im}z<K'\}.
$$

Its inverse $s(z)=\operatorname{sn}(z,k)$ maps that [rectangle](../../../geometry-and-topology.md#rectangle) onto the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), and near zero has $s(0)=0$, $s'(0)=1$. Differentiating the inverse relation gives

$$
(s')^2=(1-s^2)(1-k^2s^2),\qquad s''=-(1+k^2)s+2k^2s^3.
$$

These identities continue meromorphically.

All four [rectangle](../../../geometry-and-topology.md#rectangle) edges have real images, so [Schwarz reflection](../../../complex-analysis.md#schwarz-reflection-principle) extends $s$ across them. Reflection in the bottom edge gives $s(\bar z)=\overline{s(z)}$. Reflection in the right edge, combined with the first reflection, gives $s(2K-z)=s(z)$. The even inverse-integral [derivative](../../../calculus.md#derivative) gives $s(-z)=-s(z)$, and hence

$$
s(z+2K)=-s(z),\qquad s(z+4K)=s(z).
$$

Reflection in the top edge and then the bottom gives $s(z+2iK')=s(z)$. The resulting [period lattice of the Jacobi elliptic sine](../../../complex-analysis.md#period-lattice-of-the-jacobi-elliptic-sine) is

$$
\boxed{\Lambda=4K\mathbb Z+2iK'\mathbb Z}.
$$

To see the [poles](../../../isolated-singularity.md#pole), use $U'(w)\sim-1/(kw^2)$ near the boundary point infinity. Then $U(w)-iK'\sim1/(kw)$, so the inverse has a [simple pole](../../../isolated-singularity.md#simple-pole) at $iK'$ with [residue](../../../analysis.md#residue) $1/k$. The real half-period shift gives another [pole](../../../isolated-singularity.md#pole) at $2K+iK'$ with opposite [residue](../../../analysis.md#residue). Reflection tiles the plane with copies of the [rectangle](../../../geometry-and-topology.md#rectangle), so these are exactly two [simple poles](../../../isolated-singularity.md#simple-pole) per displayed fundamental cell. They also show there is no additional period: a period must permute these two [pole](../../../isolated-singularity.md#pole) classes; exchanging them would shift by $2K$ modulo the displayed lattice, which reverses the function's sign and [residues](../../../analysis.md#residue) rather than preserving it.

For any finite $w$, integrate $s'(z)/(s(z)-w)$ around a [fundamental parallelogram](../../../complex-analysis.md#fundamental-parallelogram-of-a-period-lattice) avoiding its zeros and [poles](../../../isolated-singularity.md#pole). The opposite edges cancel by periodicity, so the number of zeros of $s-w$ equals the number of [poles](../../../isolated-singularity.md#pole), namely two. Therefore **every value has two inverse images modulo periods, counted with multiplicity**. The value infinity likewise has the two [simple poles](../../../isolated-singularity.md#simple-pole) as preimages. Usually the finite-value preimages are distinct; the involution $z\mapsto2K-z$ interchanges them. At $w=\pm1,\pm1/k$, a critical point supplies one double inverse image instead. For example $s(K)=1$, $s'(K)=0$, $s''(K)=-(1-k^2)\ne0$. Thus the printed “exactly two” requires the standard multiplicity convention; it would be false if interpreted as two distinct solutions at these [branch values of a holomorphic map](../../../complex-analysis.md#branch-value-of-a-holomorphic-map).

Now choose $z_0=K$ and put $f(z)=s(z+K)$. Since $s(2K-z)=s(z)$, $f$ is even, elliptic for $\Lambda$, and has degree two. The [Weierstrass elliptic function](../../../complex-analysis.md#weierstrass-elliptic-function) for the same lattice is even and has one [double pole](../../../isolated-singularity.md#double-pole) per cell, hence also degree two. Its generic fibers are precisely $\{z,-z\}$. Consequently an even $f$ is constant on those fibers and descends to a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) $R$ of $\wp$. At the four fixed classes of $z\mapsto-z$, the even local Laurent expansion makes this descent [meromorphic](../../../isolated-singularity.md#meromorphic-function) in the squared local coordinate. A [meromorphic function](../../../isolated-singularity.md#meromorphic-function) on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere) is rational, so $f=R(\wp)$. Generic map degrees multiply:

$$
2=\deg f=\deg R\,\deg\wp=2\deg R.
$$

Thus $R$ has degree one and the [degree-two even elliptic function](../../../complex-analysis.md#degree-two-even-elliptic-function) conclusion is

$$
\boxed{\operatorname{sn}(z+K,k)=\frac{a\wp(z)+b}{c\wp(z)+d},\qquad ad-bc\ne0}.
$$

The [determinant](../../../linear-algebra.md#determinant) condition follows because $f$ is nonconstant. This proves the existence requested, with the explicit allowable shift $z_0=K$.

## 4

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For fixed $\operatorname{Im}\tau>0$, Gaussian decay of $|q|^{n^2}$ gives locally uniform convergence of the [theta function](../../../modular-function.md#theta-function) series and all its $z$-derivatives. It is therefore entire. Shifting the series argument and reindexing gives

$$
\theta_3(z+\pi)=\theta_3(z),\qquad
\theta_3(z+\pi\tau)=q^{-1}e^{-2iz}\theta_3(z).
$$

Since $\theta_4(z)=\theta_3(z+\pi/2)$, the corresponding second multiplier for $\theta_4$ has the opposite sign:

$$
\theta_4(z+\pi)=\theta_4(z),\qquad
\theta_4(z+\pi\tau)=-q^{-1}e^{-2iz}\theta_4(z).
$$

Thus $h=\theta_3/\theta_4$ obeys $h(z+\pi)=h(z)$ and $h(z+\pi\tau)=-h(z)$. These give candidate [period lattices](../../../complex-analysis.md#period-lattice); to show they are exact, first locate every zero.

At $z_*=(\pi+\pi\tau)/2$,

$$
\theta_3(z_*)=\sum_{n\in\mathbb Z}(-1)^nq^{n(n+1)}=0,
$$

because the terms with indices $n$ and $-n-1$ cancel. The absolute convergence justifies that pairing. Quasi-periodicity propagates this zero to every $z_*+m\pi+n\pi\tau$.

For exhaustiveness and simplicity, let $v=\theta_3'/\theta_3$. It satisfies $v(z+\pi)=v(z)$ and $v(z+\pi\tau)=v(z)-2i$. Take a [fundamental parallelogram](../../../complex-analysis.md#fundamental-parallelogram-of-a-period-lattice) for $\Lambda_0=\pi\mathbb Z+\pi\tau\mathbb Z$, translated so its boundary has no zero. The two sloping edges cancel by the first identity; the bottom and reversed top give

$$
\oint v(z)\,dz=\int_{z_0}^{z_0+\pi}\bigl(v(z)-v(z+\pi\tau)\bigr)dz=2\pi i.
$$

The [argument principle](../../../complex-analysis.md#argument-principle) therefore counts one zero with multiplicity in every cell. Since a known zero class already exists, all zeros are simple and exactly

$$
\boxed{z=\frac\pi2+\frac{\pi\tau}{2}+m\pi+n\pi\tau,\qquad m,n\in\mathbb Z}.
$$

The denominator's simple zeros are instead $\pi\tau/2+\Lambda_0$. These two cosets are disjoint: $\pi/2$ cannot lie in $\Lambda_0$ because $\operatorname{Im}\tau>0$. Thus there are no cancelled zeros or [poles](../../../isolated-singularity.md#pole) in the quotient.

Any period of $h$ or $h^2$ must translate its [zero set](../../../polynomial.md#zero-set) onto itself, so must belong to $\Lambda_0$. A translation $m\pi+n\pi\tau$ multiplies $h$ by $(-1)^n$; the quotient is nonconstant, so an odd $n$ cannot be a period of $h$. Squaring removes precisely that sign. This proves the [period lattice of theta3 over theta4](../../../modular-function.md#period-lattice-of-theta3-over-theta4) and its squared counterpart:

$$
\boxed{\operatorname{Per}\left(\frac{\theta_3}{\theta_4}\right)=\pi\mathbb Z+2\pi\tau\mathbb Z},\qquad
\boxed{\operatorname{Per}\!\left[\left(\frac{\theta_3}{\theta_4}\right)^2\right]=\pi\mathbb Z+\pi\tau\mathbb Z}.
$$

The second lattice is for the squared function; no additional translation can preserve its [zero set](../../../polynomial.md#zero-set).

## 5

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [modular group](../../../modular-function.md#modular-group) is $SL_2(\mathbb Z)$ acting on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) by

$$
\gamma\tau=\frac{a\tau+b}{c\tau+d},\qquad ad-bc=1.
$$

Its central element $-I$ acts trivially on points, so the effective group is $PSL_2(\mathbb Z)$. It is generated by $S:\tau\mapsto-1/\tau$ and $T:\tau\mapsto\tau+1$: the Euclidean algorithm reduces the bottom row of a matrix using these operations until it is a translation. The relations $S^2=(ST)^3=1$ hold in the projective group.

A [standard fundamental domain of the modular group](../../../modular-function.md#standard-fundamental-domain-of-the-modular-group) is

$$
\mathcal F=\{\tau\in\mathbb H:|\operatorname{Re}\tau|\leq1/2,\ |\tau|\geq1\}.
$$

To see that each orbit meets it, use $\operatorname{Im}(\gamma\tau)=\operatorname{Im}\tau/|c\tau+d|^2$. Choose a coprime integer pair $(c,d)$ minimizing the nonzero lattice modulus $|c\tau+d|$; a modular matrix with that bottom row maximizes the imaginary part. Translate to the central strip. If the result had modulus below one, inversion would further increase its imaginary part, a contradiction. Interior representatives are unique: for a point in the interior, $|c\tau+d|>1$ when $c\ne0$. For $|c|\geq2$ use $\operatorname{Im}\tau>\sqrt3/2$; for $|c|=1$ use the strip and the strict unit-circle bound. Thus such a matrix lowers the imaginary part, which would contradict the same fact applied to its inverse if both representatives were in the interior. Matrices with $c=0$ are translations, and cannot move one interior strip point to another.

The vertical sides are identified by $T$, and the circular halves by $S$. The exceptional points with [elliptic stabilizers of the modular group](../../../modular-function.md#elliptic-stabilizers-of-the-modular-group) are represented by $i$ and $\rho=e^{2\pi i/3}$, of projective [stabilizer](../../../group-theory.md#stabilizer-subgroup) orders two and three. The rational boundary points together with infinity form one [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) orbit. In the hyperbolic metric the region has area $\int_{-1/2}^{1/2}(1-x^2)^{-1/2}dx=\pi/3$.

A useful [subgroup](../../../group.md#subgroup) is the level-two [principal congruence subgroup](../../../group-theory.md#principal-congruence-subgroup),

$$
\Gamma(2)=\{\gamma\in SL_2(\mathbb Z):\gamma\equiv I\pmod2\}.
$$

Reduction modulo two is onto $SL_2(\mathbb F_2)$, which has six elements and permutes the three nonzero vectors. Hence its kernel has index six, and the quotient is $S_3$. In the projective action, $\Gamma(2)$ is torsion-free. Indeed finite-order nonidentity modular elements have trace zero or $\pm1$; matrices in $\Gamma(2)$ have even trace, and trace zero is impossible because $a,d$ are odd while $b,c$ are even: $ad-bc=1$ with $d=-a$ would imply $bc=-a^2-1\equiv2\pmod4$. The [subgroup](../../../group.md#subgroup) has three [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) classes, represented by $\infty,0,1$, each of width two. Parity of a primitive pair distinguishes these classes, and elementary level-two row operations reduce each class to its representative. Six translates of $\mathcal F$ supply a fundamental region. Its compactified [level-two modular curve](../../../modular-function.md#level-two-modular-curve) is obtained by adjoining these three [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) points.

Invariant [holomorphic functions](../../../complex-analysis.md#holomorphic-function) arise naturally from [theta constants](../../../modular-function.md#theta-constant). In the radian convention of Question 4, put $\Theta_j(\tau)=\theta_j(0,\tau)$, and define

$$
\lambda(\tau)=\frac{\Theta_2(\tau)^4}{\Theta_3(\tau)^4}.
$$

Here $\Theta_2=\sum_{n\in\mathbb Z}q^{(n+1/2)^2}$. The [theta-constant inversion and translation laws](../../../modular-function.md#theta-constant-inversion-and-translation-laws), obtained by Gaussian [Poisson summation](../../../fourier-analysis.md#poisson-summation-formula) and by reindexing, interchange $\Theta_2,\Theta_4$ under $S$ with the common factor $\sqrt{-i\tau}$, leave $\Theta_3$ fixed up to that factor, and under $T$ interchange $\Theta_3,\Theta_4$ while multiplying $\Theta_2$ by $e^{\pi i/4}$. Together with the [Jacobi abstruse identity](../../../modular-function.md#jacobi-abstruse-identity) $\Theta_3^4=\Theta_2^4+\Theta_4^4$, this gives

$$
\lambda(S\tau)=1-\lambda(\tau),\qquad
\lambda(T\tau)=\frac{\lambda(\tau)}{\lambda(\tau)-1}.
$$

These transformations generate the six permutations of $0,1,\infty$. In particular $T^2$ and $ST^2S^{-1}$ fix $\lambda$; with $-I$, these generate $\Gamma(2)$. Thus the [modular lambda function](../../../modular-function.md#modular-lambda-function) is invariant under this [subgroup](../../../group.md#subgroup), but not under the whole [modular group](../../../modular-function.md#modular-group). Its even [theta constants](../../../modular-function.md#theta-constant) do not vanish on $\mathbb H$, so it is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) there and avoids $0,1,\infty$. Near infinity, $\lambda=16q+O(q^2)$, with $q=e^{\pi i\tau}$, which is the width-two [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) coordinate. The two transformation laws give [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) values one at zero and infinity at one, with the same simple local orders. Thus $\lambda$ has exactly one [simple pole](../../../isolated-singularity.md#simple-pole) on the compactified level-two quotient and no [pole](../../../isolated-singularity.md#pole) in the half-plane. A [meromorphic](../../../isolated-singularity.md#meromorphic-function) map with one [simple pole](../../../isolated-singularity.md#simple-pole) has degree one, so it identifies that quotient with the sphere and the open quotient with $\mathbb C\setminus\{0,1\}$. This proves the coordinate assertion and describes all three [modular cusps](../../../modular-function.md#cusp-of-a-modular-group).

Symmetrizing this [subgroup](../../../group.md#subgroup) invariant produces a full [modular-invariant function](../../../modular-function.md#modular-invariant-function):

$$
\boxed{j(\tau)=256\frac{(1-\lambda+\lambda^2)^3}{\lambda^2(1-\lambda)^2}}.
$$

Substitution shows that this rational expression is unchanged by both $\lambda\mapsto1-\lambda$ and $\lambda\mapsto\lambda/(\lambda-1)$, hence by $S$ and $T$. It is the [Klein j-invariant](../../../modular-function.md#klein-j-invariant). Its denominator does not vanish on $\mathbb H$, so it is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) there; at the [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) it has $j\sim q^{-2}$, a [simple pole](../../../isolated-singularity.md#simple-pole) in $Q=e^{2\pi i\tau}$. It therefore remains nonconstant without being a bounded [holomorphic function](../../../complex-analysis.md#holomorphic-function) on the compactified quotient. In fact a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) invariant extending holomorphically to the compactified [modular curve](../../../modular-function.md#modular-curve) would be constant by the [maximum principle](../../../partial-differential-equation.md#maximum-principle).

This also connects invariance to [elliptic curves](../../../normalization-of-an-algebraic-curve.md#elliptic-curve): changing an oriented basis of the lattice $\mathbb Z+\tau\mathbb Z$ gives precisely the modular action after a rescaling. On the compact full modular quotient, $j$ has just the one simple [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) [pole](../../../isolated-singularity.md#pole), so its map to the sphere has degree one. It therefore classifies the resulting [homothety of complex lattices](../../../fourier-analysis.md#homothety-of-complex-lattices) classes, while the [modular lambda function](../../../modular-function.md#modular-lambda-function) retains a level-two labeling of the [branch points](../../../complex-analysis.md#branch-point) in the Legendre model $y^2=x(x-1)(x-\lambda)$. Finally, a [modular form](../../../modular-function.md#modular-form) of nonzero weight obeys a transformation law with a factor $(c\tau+d)^k$, not plain invariance; ratios of equal-weight forms instead give weight-zero [modular functions](../../../modular-function.md). The distinction between forms, invariant [holomorphic functions](../../../complex-analysis.md#holomorphic-function) on the open half-plane, and their [modular cusp](../../../modular-function.md#cusp-of-a-modular-group) behavior is essential to this construction.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
