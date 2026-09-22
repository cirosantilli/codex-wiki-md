# Paper 12

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper12.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper12.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Choose $0<R<R_1$, $0<S<S_1$ and $0<T<T_1$. On this smaller closed [polydisc](../../../complex-geometry.md#polydisc), the [holomorphic function](../../../complex-analysis.md#holomorphic-function) $A$ and its $w$-[derivative](../../../calculus.md#derivative) are bounded; write $|A|\le M$ and $|\partial_w A|\le L$. Choose $0<r<R$ with $rM<S/2$ and $rL<1$, replacing a zero bound by any positive upper bound if necessary, and choose $0<\varepsilon<T$.

Consider functions $u(z,\alpha)$ continuous on $\overline{D(0,r)}\times\overline{D(0,\varepsilon)}$, jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in the interior, with $u(0,\alpha)=0$ and $\|u\|_\infty\le S/2$. This is a closed subset of a [Banach space](../../../banach-space.md) in the supremum [norm](../../../functional-analysis.md#norm). The integral operator

$$
(\mathcal Tu)(z,\alpha)=\int_0^z A(\zeta,u(\zeta,\alpha),\alpha)\,d\zeta
$$

is well defined on the straight segment and is jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). Indeed, it equals $z\int_0^1 A(tz,u(tz,\alpha),\alpha)\,dt$, an integral of jointly [holomorphic functions](../../../complex-analysis.md#holomorphic-function) locally uniformly bounded in both variables. Convexity of the $w$-disc and the [derivative](../../../calculus.md#derivative) bound give

$$
\|\mathcal Tu\|_\infty\le rM<S/2,\qquad
\|\mathcal Tu-\mathcal Tv\|_\infty\le rL\|u-v\|_\infty.
$$

Thus the [Banach fixed-point theorem](../../../analysis.md#contraction-mapping-theorem) gives a fixed point $f(z,\alpha)$. More explicitly, the successive integral iterates starting from zero converge uniformly, and [locally uniform convergence of holomorphic functions](../../../complex-analysis.md#locally-uniform-convergence-of-holomorphic-functions) makes their limit jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). Differentiating the integral equation gives the required [complex ordinary differential equation](../../../differential-equation.md#complex-ordinary-differential-equation) and initial value. This proves **local existence, uniqueness and joint holomorphic dependence on $(z,\alpha)$**. Uniqueness among arbitrary local solutions follows first on a small disc where their values stay within $|w|<S$, by the same [contraction mapping](../../../analysis.md#contraction-mapping) estimate, and then throughout their common connected domain by the [identity theorem](../../../complex-analysis.md#identity-theorem).

For [holomorphic dependence of ordinary differential equations on parameters](../../../differential-equation.md#holomorphic-dependence-of-ordinary-differential-equations-on-parameters) in the initial value, fix an admissible initial value $w_*$ and put $u=f-w_0$. The equation becomes

$$
u'=A(z,u+w_0),\qquad u(0)=0.
$$

Its right-hand side is jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in $(z,u,w_0)$ near $(0,0,w_*)$. The preceding construction supplies a common disc and a jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) solution for $w_0$ near $w_*$. Consequently $f=u+w_0$ is jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in $z$ and its initial value $w_0$.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

**The assertion is true.** The assumed finite [multiplicity](../../../polynomial.md#multiplicity-mathematics) means that $f_0-w_1$ is not identically zero and has an isolated zero of order $k$ at $z_1$. Choose $\rho>0$ so that $\overline{D(z_1,\rho)}\subset D(0,r)$ and $f_0-w_1$ has no other zeros in this closed disc. On its boundary,

$$
\eta=\min_{|z-z_1|=\rho}|f_0(z)-w_1|>0.
$$

The joint [holomorphy](../../../complex-analysis.md#holomorphic-function) established above gives $f_\alpha\to f_0$ uniformly on that circle as $\alpha\to0$. For sufficiently small $|\alpha|$, therefore, $|f_\alpha-f_0|<\eta$. By [Rouché's theorem](../../../complex-analysis.md#rouche-s-theorem), $f_\alpha-w_1$ has exactly $k$ zeros in $D(z_1,\rho)$, counted with [multiplicity](../../../polynomial.md#multiplicity-mathematics). In particular it has at least one zero in $D(0,r)$. This preserves the total local zero count, without asserting that the zeros remain together.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

**The assertion is false for $k\ge2$, but true for $k=1$.** For $k\ge2$, take the jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) right-hand side $A_\alpha(z,w)=kz^{k-1}+\alpha$. Its solution with zero initial value is

$$
f_\alpha(z)=z^k+\alpha z=z(z^{k-1}+\alpha).
$$

At $\alpha=0$, the value zero has [multiplicity](../../../polynomial.md#multiplicity-mathematics) $k$ at the origin. For $\alpha\ne0$, however, every zero is a [simple zero](../../../complex-analysis.md#simple-zero): $f_\alpha'(0)=\alpha$, and at a nonzero zero $z^{k-1}=-\alpha$,

$$
f_\alpha'(z)=kz^{k-1}+\alpha=-(k-1)\alpha\ne0.
$$

Thus there is no zero of [multiplicity](../../../polynomial.md#multiplicity-mathematics) $k$ anywhere, even though the $k$ simple zeros stay close to zero for small $\alpha$. When $k=1$, part (a) gives exactly one zero counted with [multiplicity](../../../polynomial.md#multiplicity-mathematics) in a small disc, so that zero is simple. Alternatively, the [holomorphic implicit function theorem](../../../calculus.md#holomorphic-implicit-function-theorem) gives its [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) location as a function of $\alpha$.

## 2

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a first-order system, it is important to specify the frame in which its coefficients are written. In the simple-pole convention intended here, a [Fuchsian linear differential system](../../../differential-equation.md#fuchsian-linear-differential-system) has, at a finite singular point $a$,

$$
A(z)=\frac{R_a}{z-a}+H_a(z),\qquad H_a\text{ holomorphic near }a.
$$

The [residue](../../../analysis.md#residue) is the matrix $R_a=\lim_{z\to a}(z-a)A(z)$, computed entry by entry. Such a point is a [regular singular point](../../../complex-analysis.md#regular-singular-point): on a sector, the coefficient bound $\|A(z)\|\le C/|z-a|$ and integration along rays give at most power growth of solutions. Intrinsically, a [regular singular point](../../../complex-analysis.md#regular-singular-point) means moderate power growth of all solutions on sectors, allowing logarithmic factors. This intrinsic definition is more general than requiring a simple coefficient pole in an arbitrary meromorphic frame.

For $A(z)=R/z$, a [fundamental matrix](../../../differential-equation.md#fundamental-matrix-of-a-linear-differential-equation) on a chosen [complex logarithm](../../../analysis.md#complex-logarithm) branch is

$$
\Phi(z)=\exp(R\log z).
$$

Differentiating the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) verifies $\Phi'=R\Phi/z$. A counterclockwise circuit replaces $\log z$ by $\log z+2\pi i$, so

$$
\Phi\longmapsto\Phi M,\qquad
\boxed{M=e^{2\pi iR},\quad \text{monodromy group }=\{M^n:n\in\mathbb Z\}.}
$$

This is the [residue and monodromy of a constant Fuchsian system](../../../differential-equation.md#residue-and-monodromy-of-a-constant-fuchsian-system). A change of solution basis conjugates $M$. Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $e^{2\pi i\lambda}$ for the residue [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda$; a nontrivial [Jordan block](../../../linear-operator-theory.md#jordan-block) supplies the corresponding logarithmic terms in $z^R$. The [monodromy](../../../complex-analysis.md#monodromy) does not uniquely recover $R$, since integer shifts of residue [eigenvalues](../../../linear-operator-theory.md#eigenvalue) can leave their exponentials unchanged.

The coordinate-independent coefficient is the matrix-valued one-form $A(z)\,dz$. With $t=1/z$, its coefficient is

$$
\widetilde A(t)=-t^{-2}A(1/t).
$$

Being Fuchsian at infinity means $A(z)=O(z^{-1})$, while being ordinary there means $A(z)=O(z^{-2})$. If the finite simple poles are $a_1,\ldots,a_s$, subtract their principal parts:

$$
H(z)=A(z)-\sum_{j=1}^s\frac{R_j}{z-a_j}.
$$

Each entry of $H$ is [entire](../../../complex-analysis.md#entire-function) and tends to zero at infinity. [Liouville's theorem](../../../complex-analysis.md#liouville-theorem) therefore gives $H=0$. Expanding this [partial fraction decomposition](../../../isolated-singularity.md#partial-fraction-decomposition) at infinity yields

$$
\boxed{A(z)=\sum_{j=1}^s\frac{R_j}{z-a_j},\qquad R_\infty=-\sum_{j=1}^sR_j.}
$$

Thus the sum of all [residues](../../../analysis.md#residue), including the [residue](../../../analysis.md#residue) at infinity of the one-form, is zero. If infinity is ordinary, $R_\infty=0$ and the finite [residues](../../../analysis.md#residue) alone sum to zero. Treating $A$ merely as a scalar function of $z$, without transforming $dz$, would give the wrong infinity convention.

Put $\omega=e^{2\pi i/3}$. The possible finite singular points of $(B+zC)/(1-z^3)$ are $1,\omega,\omega^2$, and

$$
R_\zeta=-\frac{B+\zeta C}{3\zeta^2}\qquad(\zeta^3=1).
$$

A point $\zeta$ is removable exactly when $B+\zeta C=0$ as a matrix. At infinity,

$$
\widetilde A(t)=\frac{C+tB}{1-t^3},
$$

which is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) at $t=0$. Consequently **the actual set is $S=\{\zeta:\zeta^3=1,\ B+\zeta C\ne0\}$**, with $\{1,\omega,\omega^2\}$ the generic set. The finite [residues](../../../analysis.md#residue) sum to zero, as follows also from $\sum_{\zeta^3=1}\zeta^{-1}=\sum_{\zeta^3=1}\zeta^{-2}=0$.

Conversely, suppose a [Fuchsian linear differential system](../../../differential-equation.md#fuchsian-linear-differential-system) has its finite singular points among these three roots and has no singularity at infinity. Then $Q(z)=(1-z^3)A(z)$ extends to an [entire](../../../complex-analysis.md#entire-function) matrix function, and ordinariness at infinity gives $Q(z)=O(z)$. By the [Cauchy estimate](../../../analysis.md#cauchy-estimate), each entry has zero derivatives of order two or higher, so $Q(z)=B+zC$. The same argument applies to any subset $S$, with additional cancellations at the omitted roots. This proves the requested normal form.

There is a genuine convention limitation: the normal form is not true under intrinsic regular singularity alone in an unrestricted frame. For example, if $N\ne0$ and $N^2=0$, then $A(z)=N/(z-1)^2$ has [fundamental matrix](../../../differential-equation.md#fundamental-matrix-of-a-linear-differential-equation) $I-N/(z-1)$. Its solutions have only power growth, so $1$ is intrinsically a [regular singular point](../../../complex-analysis.md#regular-singular-point), and infinity is ordinary. Nevertheless its coefficient has a double pole and cannot equal $(B+zC)/(1-z^3)$. The simple-pole convention makes the preceding residue and normal-form assertions correct.

## 3

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write the [rational function](../../../isolated-singularity.md#rational-function) $A$ in reduced form. We first exclude a finite pole in its dependent variable at a generic point $(a,b)$. If this pole has order $m\ge1$, the inverse equation

$$
\frac{dz}{dw}=\frac1{A(z,w)},\qquad z(b)=a,
$$

has a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) right-hand side near $(a,b)$, with a zero of order $m$ in $w-b$ at $z=a$. Choosing a generic point avoids collisions of pole branches and zeros of the reduced numerator. The unique inverse solution has

$$
z(w)-a=c(w-b)^{m+1}+O((w-b)^{m+2}),\qquad c\ne0.
$$

To justify the leading order, first note $z'(b)=0$; if the first nonzero term has order $\ell$, substitution in the inverse equation makes the right-hand side start at order $m$, since the change caused by $z-a$ has order at least $\ell$. Thus $\ell-1=m$. Inverting produces an [algebraic branch point](../../../complex-analysis.md#algebraic-branch-point) of order $m+1$. Away from the fixed coefficient exceptions, $a$ can be chosen throughout an open set on the pole curve; inverse solutions based at these different $a$ give different initial values at a nearby ordinary point. These are [movable singularities of a complex differential equation](../../../differential-equation.md#movable-singularity-of-a-complex-differential-equation), contradicting the hypothesis. Hence the denominator has no genuine $w$-dependent factor: $A$ is a [polynomial](../../../polynomial.md) in $w$, with [rational functions](../../../isolated-singularity.md#rational-function) of $z$ as coefficients.

Let its degree in $w$ be $d$. Use the dependent coordinate $v=1/w$ on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). Its equation is

$$
v'=-v^2A(z,1/v).
$$

If $d\ge3$, the right-hand side has a pole of order $d-2$ at $v=0$ for generic $z$. The same inverse-equation argument gives a movable [algebraic branch point](../../../complex-analysis.md#algebraic-branch-point) of order $d-1$. It follows that $d\le2$, so **the equation is Riccati**, including its linear and constant special cases:

$$
\boxed{f'=a(z)f^2+b(z)f+c(z).}
$$

The requirement about the whole dependent-variable [Riemann sphere](../../../complex-analysis.md#riemann-sphere) is essential: examining only finite values would miss the branching at $f=\infty$ for degree at least three.

The [linearization of a Riccati equation](../../../analysis.md#linearization-of-a-riccati-equation) is particularly symmetric in the system

$$
\binom{f_1}{f_2}'=
\begin{pmatrix}b/2&c\\-a&-b/2\end{pmatrix}
\binom{f_1}{f_2}.
$$

On a simply connected domain where the coefficients are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point), its solutions are [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). Direct differentiation gives

$$
\left(\frac{f_1}{f_2}\right)'=
\frac{(bf_1/2+cf_2)f_2-f_1(-af_1-bf_2/2)}{f_2^2}
=a\left(\frac{f_1}{f_2}\right)^2+b\frac{f_1}{f_2}+c.
$$

A nonzero initial vector never becomes the zero vector, by uniqueness for the [linear differential equation](../../../differential-equation.md#linear-differential-equation), so the quotient is [meromorphic](../../../isolated-singularity.md#meromorphic-function). Choosing initial vector $(f(z_0),1)$ represents every finite initial value, and $(1,0)$ represents infinity. At fixed coefficient singularities, a single globally [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) vector solution need not exist; the assertion is local on ordinary domains, or on their appropriate continuation surface.

Finally, for any two finite solutions $u,v$ of the [Riccati equation](../../../analysis.md#riccati-equation),

$$
(u-v)'=(a(u+v)+b)(u-v).
$$

Use this identity on the four differences in

$$
K=\frac{(f-g)(h-j)}{(f-j)(h-g)}.
$$

The [logarithmic derivative](../../../analytic-number-theory.md#logarithmic-derivative) of this [cross-ratio](../../../group-theory.md#cross-ratio) is

$$
a(f+g+h+j-f-j-h-g)+b+b-b-b=0.
$$

Thus $K$ is constant wherever the expression is initially defined, and the identity extends as an identity of [meromorphic functions](../../../isolated-singularity.md#meromorphic-function). Distinctness of $g,h,j$ is preserved at ordinary points by uniqueness, interpreted on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). Solving the constant [cross-ratio](../../../group-theory.md#cross-ratio) equation gives the [Riccati cross-ratio superposition](../../../analysis.md#riccati-cross-ratio-superposition)

$$
\boxed{f=\frac{K(h-g)j-(h-j)g}{K(h-g)-(h-j)}.}
$$

For $K=\infty$ this means $f=j$; $K=0$ gives $g$, and $K=1$ gives $h$. The constant is selected by the initial value of $f$, so the formula represents every solution, with its denominator zeros interpreted as [poles](../../../isolated-singularity.md#pole).

## 4

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the unrestricted zero sequence, introduce the [Weierstrass elementary factors](../../../real-analysis.md#weierstrass-elementary-factor)

$$
E_p(u)=(1-u)\exp\left(u+\frac{u^2}{2}+\cdots+\frac{u^p}{p}\right).
$$

For $|u|\le1/2$, cancellation of the first $p$ terms of the logarithm [power series](../../../real-analysis.md#power-series) gives a [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm) of the factor:

$$
\log E_p(u)=-\sum_{j=p+1}^\infty\frac{u^j}{j},\qquad
|\log E_p(u)|\le2|u|^{p+1}.
$$

Define the [canonical product](../../../complex-analysis.md#canonical-product)

$$
f(z)=\prod_{n=1}^\infty E_n(z/z_n).
$$

Fix any compact disc $|z|\le R$. Since $|z_n|\to\infty$, eventually $|z/z_n|\le1/2$ uniformly on this disc. The tail logarithms are then bounded by $2(1/2)^{n+1}$, a summable bound independent of $z$. Their sum is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) by [locally uniform convergence of holomorphic functions](../../../complex-analysis.md#locally-uniform-convergence-of-holomorphic-functions), and its exponential is nowhere zero. Multiplication by the finite initial product therefore gives an [entire function](../../../complex-analysis.md#entire-function). Each factor has a [simple zero](../../../complex-analysis.md#simple-zero) exactly at its specified $z_n$, the exponential factor has none, and a tail beginning beyond any given compact disc is nonvanishing there. Thus **$f$ has precisely the prescribed zeros and no others**, each simple, and $f(0)=1$. This proves the required existence without an assumption on $\sum_n|z_n|^{-1}$.

For the final, unheaded product request, suppose now that $\sum_n|z_n|^{-1}<\infty$. On $|z|\le R$, all sufficiently late factors have $|z/z_n|\le1/2$, so part (a) bounds their [principal complex logarithms](../../../analysis.md#principal-complex-logarithm) by $2R/|z_n|$. The logarithms converge absolutely and uniformly; [infinite product convergence from logarithmic tails](../../../real-analysis.md#infinite-product-convergence-from-logarithmic-tails) proves that

$$
P(z)=\prod_{n=1}^\infty(1-z/z_n)
$$

is [entire](../../../complex-analysis.md#entire-function) and again has exactly the prescribed simple zeros. For its finite partial products,

$$
\prod_{n=1}^N|1-z/z_n|
\le\prod_{n=1}^N(1+|z|/|z_n|)
\le\exp\left(|z|\sum_{n=1}^N|z_n|^{-1}\right).
$$

Passing to the limit proves

$$
\boxed{|P(z)|\le e^{C|z|},\qquad C=\sum_{n=1}^\infty|z_n|^{-1}<\infty.}
$$

In particular $P$ is an [entire function of exponential type](../../../complex-analysis.md#entire-function-of-exponential-type). This argument uses a valid modulus estimate and does not require the false logarithm assertion in part (c).

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $|w|\le1/2$, the [power series](../../../real-analysis.md#power-series) of the [principal complex logarithm](../../../analysis.md#principal-complex-logarithm) is absolutely convergent and gives

$$
|\operatorname{Log}(1-w)|
\le\sum_{j=1}^\infty\frac{|w|^j}{j}
\le\sum_{j=1}^\infty|w|^j
=\frac{|w|}{1-|w|}
\le2|w|.
$$

Thus **$C_1=2$ works**. The value $1-w$ stays in the right half-plane, so there is no logarithm branch ambiguity. This is the [bounds for the principal logarithm near one](../../../analysis.md#bounds-for-the-principal-logarithm-near-one) estimate used to control product tails.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For every real $r\ge0$,

$$
\log(1+r)=\int_0^r\frac{dt}{1+t}\le r.
$$

Taking $r=|w|$ proves the required [logarithm inequality](../../../calculus.md#logarithm-inequality), even without the lower bound $|w|\ge1/2$. Hence **$C_2=1$ works**.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

**The printed assertion is false.** Take real $w=1-\varepsilon$ with $0<\varepsilon<1$. The [principal complex logarithm](../../../analysis.md#principal-complex-logarithm) is unambiguous, but

$$
|\operatorname{Log}(1-w)|=|\log\varepsilon|\longrightarrow\infty,
\qquad |w|\longrightarrow1.
$$

No finite $C_3$ can satisfy the proposed estimate, even on these points within the logarithm's domain. At $w=1$ the logarithm is undefined, and the usual principal analytic branch also excludes its cut. These are additional reasons the literal all-$w$ assertion cannot hold.

The valid estimate for the final product proof is instead

$$
\log|1-w|\le\log(1+|w|)\le|w|\qquad(w\ne1),
$$

or equivalently $|1-w|\le e^{|w|}$ for every $w$, including $w=1$. The upper bound on the real part of the logarithm is enough for growth; a bound on the full modulus of the logarithm is unnecessary. The preceding root Solution supplies the complete convergence and exponential-growth proof using this correction.

## 5

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Write $\log^+x=\max(0,\log x)$. The [Nevanlinna proximity function](../../../isolated-singularity.md#nevanlinna-proximity-function) and [Nevanlinna integrated counting function](../../../isolated-singularity.md#nevanlinna-integrated-counting-function) are

$$
m(r,f)=\frac1{2\pi}\int_0^{2\pi}\log^+|f(re^{i\theta})|\,d\theta,
\qquad
N(r,f)=\sum_{|p_n|<r}\log\frac r{|p_n|}.
$$

The pole sum counts [multiplicity](../../../polynomial.md#multiplicity-mathematics); it is finite for each $r$ because $f(0)$ is finite and nonzero and [poles](../../../isolated-singularity.md#pole) of a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) are isolated. Equivalently $N(r,f)=\int_0^r n(t,f)\,dt/t$, where $n(t,f)$ counts poles in the disc. The [Nevanlinna characteristic](../../../isolated-singularity.md#nevanlinna-characteristic) is

$$
\boxed{T(r,f)=m(r,f)+N(r,f).}
$$

For a general nonzero [meromorphic function](../../../isolated-singularity.md#meromorphic-function) $g$ with signed order $\nu$ at zero, use $g(z)=cz^\nu(1+O(z))$, $c\ne0$. The general counting convention includes a pole at zero:

$$
N(r,g)=n(0,g)\log r+\int_0^r\frac{n(t,g)-n(0,g)}t\,dt,
$$

where $n(0,g)=\max(0,-\nu)$. This convention will also cover $g=f-a$ when the target $a=f(0)$.

Here is a direct proof of the exact reciprocal identity underlying the [Nevanlinna first main theorem](../../../isolated-singularity.md#nevanlinna-first-main-theorem). Choose a circle with no zero or pole of $g$ on it, and a slightly larger disc with the same interior zeros and poles. Divide $g$ by $z^\nu$ and its nonzero zero factors and multiply by its nonzero pole factors, obtaining a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point), nowhere-zero function $H$ on that disc. For any factor $z-a$ with $|a|<r$,

$$
\frac1{2\pi}\int_0^{2\pi}\log|re^{i\theta}-a|\,d\theta=\log r.
$$

Indeed, factor out $re^{i\theta}$; the remaining logarithm has real part equal to that of $-\sum_{k\ge1}(a/r)^ke^{-ik\theta}/k$, whose angular mean is zero. Also, $\log|H|$ is [harmonic](../../../partial-differential-equation.md#harmonic-function), so the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) equates its circle mean to $\log|H(0)|$. Putting back the zero and pole factors proves

$$
\frac1{2\pi}\int_0^{2\pi}\log|g(re^{i\theta})|\,d\theta
=\log|c|+N(r,1/g)-N(r,g).
$$

The identity $\log^+x-\log^+(1/x)=\log x$ now yields

$$
\boxed{T(r,g)-T(r,1/g)=\log|c|.}
$$

Zeros or poles on the circle cause only integrable logarithmic singularities; the same identities hold at those radii by limits. A boundary zero or pole contributes $\log(r/r)=0$ to its counting term.

For a finite target $a$, set $g=f-a$. Its finite [poles](../../../isolated-singularity.md#pole) and their orders equal those of $f$. The elementary estimates

$$
\log^+|f-a|\le\log^+|f|+\log(1+|a|),\qquad
\log^+|f|\le\log^+|f-a|+\log(1+|a|)
$$

give $|T(r,f-a)-T(r,f)|\le\log(1+|a|)$. Combining this with the reciprocal identity proves **the first main theorem**:

$$
\boxed{T(r,f)=m(r,1/(f-a))+N(r,1/(f-a))+O(1).}
$$

The error is bounded independently of $r$, with an explicit bound $\log(1+|a|)+|\log|c_a||$, where $c_a$ is the first nonzero local coefficient of $f-a$ at zero. The count on the right records the occurrences of the value $a$ with [multiplicity](../../../polynomial.md#multiplicity-mathematics). The target infinity is the defining identity $T=m+N$. If $f$ is a constant equal to $a$, the reciprocal expression is undefined; the value-distribution assertion assumes $f-a\not\equiv0$, as it automatically does for nonconstant $f$. The exact reciprocal identity remains valid for every nonzero constant $f$.

Taking $g=f$, whose signed order is zero and whose local coefficient is $f(0)$, rearranges that exact identity into [Jensen's formula](../../../complex-analysis.md#jensen-s-formula):

$$
\boxed{\frac1{2\pi}\int_0^{2\pi}\log|f(re^{i\theta})|\,d\theta
=\log|f(0)|+
\sum_{|z_n|<r}\log\frac r{|z_n|}
-\sum_{|p_n|<r}\log\frac r{|p_n|}.}
$$

Thus the zero and pole terms, their signs and the initial-value constant follow from the same proved identity, rather than from a theorem citation without proof.

Finally let $f$ be a nonzero bounded [holomorphic function](../../../complex-analysis.md#holomorphic-function) on the [unit disc](../../../topology.md#unit-disc), with $|f|\le M$. If its order at zero is $m$, write $f(z)=z^m h(z)$, $h(0)\ne0$. The factorization argument above works on every compact subdisc and gives, for its nonzero zeros,

$$
\sum_{0<|z_n|<r}\log\frac r{|z_n|}
\le\log M-\log|h(0)|-m\log r.
$$

For $1/2\le r<1$ this is a uniform finite upper bound. As $r\uparrow1$, [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) gives

$$
\sum_{z_n\ne0}\log\frac1{|z_n|}<\infty.
$$

Since $1-u\le-\log u$ for $0<u<1$, and there are only $m$ zeros at zero, we obtain

$$
\boxed{\sum_n(1-|z_n|)<\infty.}
$$

This is precisely the [Blaschke condition](../../../complex-analysis.md#blaschke-condition), so the zeros, counted with [multiplicity](../../../polynomial.md#multiplicity-mathematics), form a [Blaschke sequence](../../../complex-analysis.md#blaschke-sequence).

## 6

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [fixed singularity of a complex differential equation](../../../differential-equation.md#fixed-singularity-of-a-complex-differential-equation) has a location determined by the coefficients, independently of the initial value. A [movable singularity of a complex differential equation](../../../differential-equation.md#movable-singularity-of-a-complex-differential-equation) belongs to an individual continued solution and changes location when the initial value changes. For example, $w'=w^2$ has the movable [pole](../../../isolated-singularity.md#pole) $z=c$ in $w=-1/(z-c)$. A fixed exceptional location need not be singular for every solution.

The precise first-order form of the [Painlevé determinateness theorem](../../../differential-equation.md#painleve-determinateness-theorem) needed here is as follows. Let $w'=A(z,w)$ be rational in $w$, with coefficients [meromorphic](../../../isolated-singularity.md#meromorphic-function) in $z$ on the chosen independent-variable surface. Algebraic coefficients can be made single valued on their own surface. Exclude the fixed coefficient singularities and exceptional fibres where a reduced numerator and denominator vanish together, working also in the dependent coordinate $v=1/w$. If a solution is continued along an arc $\gamma:[0,1)\to U$ with endpoint $z_*=\lim_{t\to1}\gamma(t)$ outside that exceptional set, then **$w(\gamma(t))$ has a definite finite or infinite limit**. Any singularity there is a [pole](../../../isolated-singularity.md#pole) or an [algebraic branch point](../../../complex-analysis.md#algebraic-branch-point); there is no movable essential or logarithmic singularity. The standard rectifiable-arc formulation is included in this statement.

Here is a proof. First suppose a sequence along the arc has $(z_n,w_n)\to(z_*,w_*)$ at a point where the vector field is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point). Choose a smaller closed bidisc about this point. Uniform bounds on the vector field and its dependent-variable [derivative](../../../calculus.md#derivative) give, by the integral [contraction mapping](../../../analysis.md#contraction-mapping) proof, one radius $r>0$ on which every solution starting sufficiently close to $(z_*,w_*)$ exists and remains bounded. For large $n$, the solution through $(z_n,w_n)$ is therefore defined on a fixed disc about $z_*$. The entire sufficiently late tail of $\gamma$ lies in that disc. Uniqueness identifies the original continued solution with this local solution throughout that tail, so the solution extends through $z_*$ and has a limit. The same argument applies to an ordinary point in the reciprocal coordinate $v=1/w$.

If the limit did not exist, consider the cluster set $K$ in the dependent-variable [Riemann sphere](../../../complex-analysis.md#riemann-sphere):

$$
K=\bigcap_{s<1}\overline{\{w(\gamma(t)):s\le t<1\}}.
$$

Each closed tail is compact and connected, and these sets are nested; hence $K$ is nonempty, compact and connected. The preceding paragraph excludes every ordinary point from $K$. At $z_*$ the rational vector field has only finitely many nonordinary dependent values, in both coordinate charts: an entire fibre of singular points was excluded among the fixed exceptions. Thus $K$ is a connected subset of a finite set, so it is a singleton. Compactness then forces convergence to its unique point, contradicting the assumed lack of a limit. This proves determinateness.

It remains to determine the local type rather than merely the limit. At a finite limiting value $w_*$ which is a pole of the vector field, write the reduced equation as $w'=P/Q$. Since $z_*$ is not exceptional, $P(z_*,w_*)\ne0$, and the inverse equation

$$
\frac{dz}{dw}=\frac{Q(z,w)}{P(z,w)}
$$

is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) near $(z_*,w_*)$. The [holomorphic dependence of ordinary differential equations on parameters](../../../differential-equation.md#holomorphic-dependence-of-ordinary-differential-equations-on-parameters) makes its local solution curves jointly [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) in $w$ and their initial $z$ values. In particular, the value at the transverse line $w=w_*$ is a [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) first integral labelling these curves. The original graph has constant label; taking its endpoint limit shows that it lies on the inverse solution through $(z_*,w_*)$. That inverse solution cannot be the vertical curve $z\equiv z_*$: this would require $Q(z_*,w)$ to vanish identically near $w_*$, an excluded fixed singular fibre. Consequently its [power series](../../../real-analysis.md#power-series) has a first nonzero term,

$$
z(w)-z_*=c(w-w_*)^k+O((w-w_*)^{k+1}),\qquad c\ne0.
$$

Here $k\ge2$ at a vector-field pole. Factor the right side as $(w-w_*)^k$ times a nonvanishing [holomorphic function](../../../complex-analysis.md#holomorphic-function) and take its local $k$th root. This gives a new dependent coordinate with nonzero [derivative](../../../calculus.md#derivative), and the [holomorphic inverse function theorem](../../../geometry-and-topology.md#holomorphic-inverse-function-theorem) expresses $w$ as a convergent [power series](../../../real-analysis.md#power-series) in $(z-z_*)^{1/k}$. Thus the singularity is an [algebraic branch point](../../../complex-analysis.md#algebraic-branch-point). At an infinite limit, repeat the argument for $v=1/w$. An ordinary zero of $v$ gives a [pole](../../../isolated-singularity.md#pole) of $w$, while a finite ramification of $v$ gives an algebraic pole branch. This proves the asserted local types and the theorem.

For the given equation, the finite-coordinate rational field is

$$
A(z,w)=\frac{w}{(z+1)(w^2-z^2)}.
$$

The whole fibre $z=-1$ is singular in the displayed coefficient, and at $(z,w)=(0,0)$ the reduced numerator and denominator vanish together. Hence the finite fixed exceptional set is $\{-1,0\}$. Away from these two locations, the only possible finite dependent limits at a singularity are $w_* =\sigma z_*$, with $\sigma=\pm1$.

At such a point the inverse equation is

$$
z_w=\frac{(z+1)(w^2-z^2)}w.
$$

It is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) when $z_*\ne0,-1$ and $w_* =\sigma z_*$. Its inverse solution satisfies $z_w(w_*)=0$, and differentiation gives

$$
z_{ww}(w_*)=(z_*+1)\left(1+\frac{z_*^2}{w_*^2}\right)=2(z_*+1).
$$

Therefore

$$
z-z_*=(z_*+1)(w-w_*)^2+O((w-w_*)^3),
$$

and

$$
\boxed{w(z)=\sigma z_*\;\pm\sqrt{\frac{z-z_*}{z_*+1}}+O(z-z_*).}
$$

These are genuine square-root [algebraic branch points](../../../complex-analysis.md#algebraic-branch-point). The inverse solutions can be based at arbitrary $z_*\notin\{0,-1\}$ and then continued to nearby ordinary initial points. Their distinct branch locations require different initial data, so **these branch points are movable**. The signs specify the two inverse branches near each of the two values $w_* =\pm z_*$.

There are **no movable poles**. Indeed the reciprocal equation is

$$
v'=-\frac{v^3}{(z+1)(1-z^2v^2)}.
$$

For every finite $z\ne-1$ it is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) at $v=0$, and $v\equiv0$ is its unique solution with zero initial value. A nonzero reciprocal solution therefore cannot reach zero there. This rules out both an ordinary pole and an infinite algebraic branch at a movable finite location. Together with the theorem, it exhausts the finite movable singularities.

The fixed point zero must not be mistaken for a generic movable collision. It is ordinary for solutions with $w(0)\ne0$. But solutions reaching $w=0$ can have a fixed square-root singularity. To construct them rather than just balance powers, set $z(w)=w^2h(w)$ in the inverse equation. The equation for $h$ is

$$
wh'=1-2h+w^2(h-h^2)-w^4h^3,\qquad h(0)=\tfrac12.
$$

Equivalently,

$$
h(w)=\int_0^1t\left[1+w^2t^2\{h(wt)-h(wt)^2\}-w^4t^4h(wt)^3\right]dt.
$$

On a small disc this is a [contraction mapping](../../../analysis.md#contraction-mapping) of the closed ball $\|h-1/2\|_\infty\le1/4$: both its departure from $1/2$ and its Lipschitz constant are $O(r^2)$. Its unique [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) fixed point gives $z=w^2/2+O(w^4)$. Thus

$$
w(z)=\pm\sqrt{2z}\,(1+O(z))
$$

is a genuine branch at the fixed location zero. The zero solution itself extends through zero as a function, although the original displayed coefficient is undefined at $(0,0)$.

The point $-1$ can produce a fixed nonalgebraic singularity. For an explicit example take $z=-1+x$ real, $0<x<x_0<1$, and $w=iy$ with initial $y>2$. Put $q=y^2$ and $L=-\log x$. Then

$$
\frac{dq}{dL}=\frac{2q}{q+(x-1)^2}.
$$

As $L$ increases, $q$ increases, its derivative is bounded above by $2$ and bounded below by a positive constant, and therefore the solution exists for all large $L$ and $q\to\infty$. The derivative then tends to $2$, so $q/L\to2$. Consequently

$$
w(z)^2\sim2\log(z+1)\qquad(z\downarrow-1).
$$

This is unbounded but grows more slowly than every negative power of $z+1$. It cannot be a meromorphic pole even after a finite ramified substitution, demonstrating an actual fixed singularity with logarithmic growth. The determinateness theorem does not exclude such behavior at fixed exceptions.

Finally, on the independent-variable [Riemann sphere](../../../complex-analysis.md#riemann-sphere) use $t=1/z$. For finite $w$ the transformed equation is

$$
\frac{dw}{dt}=\frac{tw}{(1+t)(1-t^2w^2)},
$$

which is ordinary at $t=0$. At simultaneous $z=\infty$, $w=\infty$, however, the reciprocal field is

$$
\frac{dv}{dt}=-\frac{tv^3}{(1+t)(v^2-t^2)},
$$

with an indeterminate point at $(t,v)=(0,0)$. Thus infinity is an additional fixed exceptional location on the sphere, rather than an unavoidable singularity of solutions with finite limiting value. There are solutions escaping to infinity there: for real initial data $w(z_0)>z_0>0$, the difference $d=w-z$ stays positive, since its derivative becomes positive as $d\downarrow0$. Moreover $d'\le0$ when $d\ge1$, so $0<d\le\max(1,d(z_0))$. Such a solution continues for all positive $z$, with $w=z+O(1)\to\infty$.

**In the finite plane, the fixed exceptional locations are $0,-1$; all other solution singularities are movable square-root branches at $w=\pm z$, and there are no movable poles. On the sphere, infinity is also a fixed exception at the infinite dependent value.** Being fixed or movable describes the base location, not merely whether the coefficient contains the factors $w-z$ and $w+z$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
