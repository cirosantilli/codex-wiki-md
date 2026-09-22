# Paper 9

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_9.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_9.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Weak Harnack inequality](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality) is an estimate for a nonnegative [weak supersolution](../../../elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation). Write $F=(f^1,\ldots,f^n)$, let $B_{2R}(x_0)\subset\subset\Omega$, and assume $u\geq0$ almost everywhere on this ball. There are $p>0$ and $C<\infty$, depending only on the dimension, the [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) bounds, $q$, and the scaled norms of the lower-order coefficients, such that

$$
\boxed{\left(\frac{1}{|B_R(x_0)|}\int_{B_R(x_0)}u^p\right)^{1/p}\leq C\left(\operatorname*{ess\,inf}_{B_R(x_0)}u+R^{1-n/q}\|F\|_{L^q(B_{2R})}+R^{2-2n/q}\|g\|_{L^{q/2}(B_{2R})}\right).}
$$

Here $\langle v\rangle_E=|E|^{-1}\int_Ev$ is the [integral average](../../../measure-theory.md#integral-average). The [weak supersolution](../../../elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation) inequality uses the sign convention $Lu\leq\operatorname{div}F+g$. For instance, the coefficient dependence can be expressed using

$$
R^{1-n/q}(\|b\|_{L^q(B_{2R})}+\|c\|_{L^q(B_{2R})}),\qquad R^{2-2n/q}\|d\|_{L^{q/2}(B_{2R})}.
$$

Thus one may use the same $p,C$ on all sufficiently small balls when the global coefficient norms and [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) bounds are fixed. The nonnegativity condition is essential to this formulation; a signed [weak supersolution](../../../elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation) may first be shifted, with the resulting change in its forcing included. As usual, supremum and infimum statements for functions in a [Sobolev space](../../../sobolev-space.md) mean [essential suprema](../../../measure-theory.md#essential-supremum) and [essential infima](../../../real-analysis.md#essential-infimum). The standard multidimensional statement uses $n\geq2$, so $q/2>1$. In dimension one the analogous formulation requires $q\geq2$; the printed restriction $q>n$ alone would allow $q/2<1$, which does not suffice. To see the obstruction, smooth the nonnegative capped function $\min\{1,|x|/\varepsilon\}$ by a [mollifier](../../../distribution-theory.md#mollifier) of width $\tau$. Its positive second derivative is a bump of mass $2/\varepsilon$ and has $L^{q/2}$ size of order $\varepsilon^{-1}\tau^{2/q-1}$. For fixed $\varepsilon$ and $1<q<2$, this size and the minimum both tend to zero as $\tau\downarrow0$, whereas the average on a fixed larger interval stays positive. Thus the [Weak Harnack inequality](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality) cannot have the displayed uniform forcing bound in that range. Shrinking $\varepsilon$ and choosing $\tau$ still smaller likewise defeats a uniform Hölder estimate based on that norm alone.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $M=\operatorname*{ess\,sup}_{\Omega}u$. The standard [local boundedness of weak elliptic subsolutions](../../../elliptic-boundary-value-problem.md#local-boundedness-of-weak-elliptic-subsolutions) gives a finite upper bound on every [relatively compact](../../../topological-analysis.md#relatively-compact-subset) ball. In particular, the assumed equality of [essential suprema](../../../measure-theory.md#essential-supremum) makes $M$ finite. Equivalently, when using the maximum principle for an upper-bounded [weak subsolution](../../../elliptic-boundary-value-problem.md#weak-subsolution-of-a-divergence-form-elliptic-equation), this preliminary fact is already part of the hypothesis.

Set $v=M-u$. Because the [divergence-form elliptic operator](../../../elliptic-boundary-value-problem.md#divergence-form-elliptic-operator) here annihilates constants, $v\geq0$ and $Lv=-Lu\leq0$. The hypothesis says $\operatorname*{ess\,inf}_Bv=0$. Cover the compact closure of $B$ by finitely many balls $D_j$ whose doubled balls lie in $\Omega$. At least one $D_j$ has [essential infimum](../../../real-analysis.md#essential-infimum) zero: otherwise the minimum of their finitely many positive lower bounds would be a positive lower bound on $B$. The [Weak Harnack inequality](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality) with zero forcing now gives

$$
\left(\frac{1}{|D_j|}\int_{D_j}v^p\right)^{1/p}\leq C\operatorname*{ess\,inf}_{D_j}v=0.
$$

Consequently $v=0$ almost everywhere on $D_j$. If another admissible ball overlaps $D_j$ in an open set, its [essential infimum](../../../real-analysis.md#essential-infimum) of $v$ is also zero, and the same argument makes $v$ vanish there. Since a domain is [connected](../../../geometry-and-topology.md#connected-space), a chain of overlapping interior balls reaches every point of $\Omega$. This [propagation of zeros by the weak Harnack inequality](../../../elliptic-boundary-value-problem.md#propagation-of-zeros-by-the-weak-harnack-inequality) proves **$u=M$ almost everywhere on $\Omega$**, which is the claimed [strong maximum principle](../../../elliptic-boundary-value-problem.md#strong-maximum-principle-for-elliptic-operators). Notice why the absence of the $b,d$ terms matters: it is precisely what makes $L(M-u)=-Lu$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Put $\alpha=1-n/q>0$ and

$$
A=\operatorname*{ess\,sup}_{\Omega}|u|,\qquad N=A+\|F\|_{L^q(\Omega)}+\|g\|_{L^{q/2}(\Omega)}.
$$

First suppose $A<\infty$. For an interior ball $B_R$, with $R\leq1$, write $M_R=\operatorname*{ess\,sup}_{B_R}u$, $m_R=\operatorname*{ess\,inf}_{B_R}u$, and $\omega(R)=M_R-m_R$. Constant shifts of a [divergence-form elliptic operator](../../../elliptic-boundary-value-problem.md#divergence-form-elliptic-operator) change its forcing. The two nonnegative [weak supersolutions](../../../elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation) $v=M_R-u$ and $w=u-m_R$ satisfy, respectively,

$$
Lv=\operatorname{div}(M_Rb-F)+(M_Rd-g),\qquad Lw=\operatorname{div}(F-m_Rb)+(g-m_Rd).
$$

Their [Weak Harnack inequalities](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality) on $B_{R/2}$ therefore have forcing errors bounded by $CNR^\alpha$. Indeed $|M_R|,|m_R|\leq A$, the new divergence forcing is bounded by $\|F\|_q+A\|b\|_q$, and the scalar forcing by $\|g\|_{q/2}+A\|d\|_{q/2}$; also $R^{2\alpha}\leq R^\alpha$.

On $B_{R/2}$ we have $v+w=\omega(R)$. Even if $p<1$, the elementary inequality $(s+t)^p\leq C_p(s^p+t^p)$ implies

$$
\omega(R)\leq C_p\left(\left(\frac{1}{|B_{R/2}|}\int_{B_{R/2}}v^p\right)^{1/p}+\left(\frac{1}{|B_{R/2}|}\int_{B_{R/2}}w^p\right)^{1/p}\right).
$$

The sum of the two [essential infima](../../../real-analysis.md#essential-infimum) is $\omega(R)-\omega(R/2)$. Enlarging a uniform constant $C_0>1$ gives

$$
\omega(R)\leq C_0\bigl(\omega(R)-\omega(R/2)+CNR^\alpha\bigr),\qquad \omega(R/2)\leq\theta\omega(R)+CNR^\alpha,
$$

where $\theta=1-C_0^{-1}\in(0,1)$. This is an [oscillation decay estimate](../../../elliptic-boundary-value-problem.md#oscillation-decay-estimate); [inhomogeneous oscillation decay implies Hölder continuity](../../../elliptic-boundary-value-problem.md#inhomogeneous-oscillation-decay-implies-holder-continuity). Choose

$$
0<\mu<\min\{\alpha,-\log_2\theta,1\}.
$$

Iterating on concentric balls, starting at a fixed admissible radius $R_*\leq1$, yields

$$
\omega(2^{-k}R_*)\leq\theta^k\omega(R_*)+CN R_*^\alpha\sum_{j=0}^{k-1}\theta^j2^{-\alpha(k-1-j)}\leq C N2^{-k\mu}.
$$

The strict choice of $\mu$ bounds the [geometric series](../../../real-analysis.md#geometric-series), including the case in which the two original decay rates coincide. Monotonicity of oscillation extends this bound to intermediate radii.

Take $R_*$ uniformly smaller than the distance of $\Omega'$ from the boundary of $\Omega$. The vanishing essential oscillation produces a continuous representative of $u$. A ball centred at either of two sufficiently close points of $\Omega'$ contains both, so its oscillation bounds their difference by $CN|x-y|^\mu$. For separated points use $|u(x)-u(y)|\leq2A$. Thus the [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) satisfies

$$
\boxed{[u]_{\mu;\Omega'}\leq C\left(\operatorname*{ess\,sup}_{\Omega}|u|+\|F\|_{L^q(\Omega)}+\|g\|_{L^{q/2}(\Omega)}\right).}
$$

The constants depend only on the indicated domain separation, dimension, coefficient norms, [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) bounds and $q$. If the global [essential supremum](../../../measure-theory.md#essential-supremum) is infinite, the displayed global estimate is vacuous; [local boundedness of weak elliptic subsolutions](../../../elliptic-boundary-value-problem.md#local-boundedness-of-weak-elliptic-subsolutions) on slightly larger compact subsets still makes the same argument prove interior [Hölder continuity](../../../sobolev-space.md#holder-condition).

## 2

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a bounded domain, the [nondivergence-form elliptic operator](../../../elliptic-boundary-value-problem.md#nondivergence-form-elliptic-operator) obeys the [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators): $Lu\geq0$ and $c\leq0$ imply

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}=\sup_{\partial\Omega}u^+.}
$$

Here $u^+=\max\{u,0\}$. Boundedness of $\Omega$ is needed for this formulation: it is not explicitly imposed in this question. On an unbounded domain one needs an appropriate condition at infinity instead. Without either condition the claim is false, as $u(x)=x_n$ and $L=\Delta$ on the half-space $\{x_n>0\}$ show.

For the bounded-domain proof choose $\gamma>0$ so large that $\lambda\gamma^2-\|b^1\|_\infty\gamma-\|c\|_\infty>0$. The positive exponential $h(x)=e^{\gamma x_1}$ then satisfies

$$
Lh=e^{\gamma x_1}\bigl(\gamma^2a^{11}+\gamma b^1+c\bigr)>0.
$$

Let $u_\varepsilon=u+\varepsilon h$, $M=\sup_{\partial\Omega}u^+$ and $H=\sup_{\overline\Omega}h<\infty$. If $u_\varepsilon$ had a value greater than $M+\varepsilon H$, it would attain a positive maximum at an interior point. There its [gradient](../../../calculus.md#gradient) vanishes and its [Hessian matrix](../../../calculus.md#hessian-matrix) is [negative semidefinite](../../../calculus.md#negative-semidefinite-matrix). The symmetric part of $(a^{ij})$ is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) by [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator), so $a^{ij}D_{ij}u_\varepsilon\leq0$; also $cu_\varepsilon\leq0$. Hence $Lu_\varepsilon\leq0$, contradicting $Lu_\varepsilon=Lu+\varepsilon Lh>0$. Thus $u_\varepsilon\leq M+\varepsilon H$. Letting $\varepsilon\downarrow0$ proves the [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators), without requiring continuity of the coefficients.

For example, the unbounded-domain version follows by exhausting the domain with bounded truncations if $\limsup_{|x|\to\infty,\,x\in\Omega}u(x)\leq M$: the added spherical boundaries then have supremum at most $M+o(1)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In the bounded-domain setting of the [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators), let $u_1,u_2$ be two [classical solutions](../../../partial-differential-equation.md#classical-solution) with the same forcing and boundary values. Their difference $z=u_1-u_2$ satisfies $Lz=0$ and $z=0$ on the boundary. Apply the [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) first to $z$ and then to $-z$:

$$
\sup_\Omega z\leq0,\qquad\sup_\Omega(-z)\leq0.
$$

Thus **$u_1=u_2$**, proving uniqueness of the [Dirichlet problem](../../../analysis.md#dirichlet-problem). The same proof works on an unbounded domain if the difference and its negative satisfy the required condition at infinity. As literally printed without either restriction, uniqueness need not hold: on $\{x_n>0\}$ the two [harmonic functions](../../../partial-differential-equation.md#harmonic-function) $0$ and $x_n$ have the same zero boundary values.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

On the unit ball take the [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) $L=\Delta-2n$ and the smooth function $u(x)=-1-|x|^2$. The zeroth-order coefficient is negative and

$$
Lu=-2n+2n(1+|x|^2)=2n|x|^2\geq0.
$$

Nevertheless

$$
\boxed{\sup_{B_1}u=-1>-2=\sup_{\partial B_1}u.}
$$

This is consistent with the [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators), whose upper bound here is $\sup_{\partial B_1}u^+=0$. At a negative interior maximum the term $cu$ can be positive; this is why a negative boundary maximum cannot replace its [positive part](../../../function.md#positive-part-of-a-real-valued-function). If $c=0$, subtracting the boundary maximum preserves the differential inequality and gives the stronger bound. That subtraction is unavailable for general $c\leq0$.

## 3

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use a [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) [cutoff function](../../../distribution-theory.md#cutoff-function) $\eta$ which equals one on $B_R(x_0)$, vanishes outside $B_{2R}(x_0)$, takes values in $[0,1]$, and has $|\nabla\eta|\leq2/R$. Its [gradient](../../../calculus.md#gradient) is supported in the [annulus](../../../topology.md#annulus-mathematics) $A_R=B_{2R}(x_0)\setminus B_R(x_0)$. The function $\eta^2(u-c)$ is an admissible [test function](../../../distribution-theory.md#test-function) in the zero-boundary [Sobolev space](../../../sobolev-space.md) for the [weak solution](../../../partial-differential-equation.md#weak-solution), by approximation with smooth compactly supported [test functions](../../../distribution-theory.md#test-function). If $\Lambda_0$ bounds the [operator norm](../../../continuous-dual-space.md#operator-norm) of $(a^{ij})$, we can take $\Lambda_0=n\Lambda$. The weak equation and [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) give

$$
\lambda\int\eta^2|\nabla u|^2\leq2\Lambda_0\int_{A_R}\eta|\nabla u|\,|u-c|\,|\nabla\eta|.
$$

[Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) bounds the right side by

$$
\frac\lambda2\int\eta^2|\nabla u|^2+\frac{2\Lambda_0^2}{\lambda}\int_{A_R}|u-c|^2|\nabla\eta|^2.
$$

After absorption, this [annular Caccioppoli inequality](../../../partial-differential-equation.md#annular-caccioppoli-inequality) is

$$
\boxed{\int_{B_R(x_0)}|\nabla u|^2\leq\frac{16\Lambda_0^2}{\lambda^2R^2}\int_{A_R}|u-c|^2.}
$$

The dimension is fixed in the notation $C(\lambda,\Lambda)$ of the question; with the entrywise coefficient bound its dependence on $n$ is absorbed there. If the larger ball merely lies in $B$ without its closure being compactly contained, approximation from smaller [cutoff functions](../../../distribution-theory.md#cutoff-function) gives the same admissible [test function](../../../distribution-theory.md#test-function) and estimate. Crucially, the right side uses only the [annulus](../../../topology.md#annulus-mathematics), where the [cutoff function](../../../distribution-theory.md#cutoff-function) varies. The constant $c$ is arbitrary because constants have zero [gradient](../../../calculus.md#gradient).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $E(t)=\int_{B_t(x_0)}|\nabla u|^2$. For $n\geq2$, choose $c$ in the [annular Caccioppoli inequality](../../../partial-differential-equation.md#annular-caccioppoli-inequality) to be the [integral average](../../../measure-theory.md#integral-average) of $u$ over $A_R$. The supplied [Poincare inequality on an annulus](../../../sobolev-space.md#poincare-inequality-on-an-annulus) gives

$$
E(R)\leq C_1R^{-2}\int_{A_R}|u-c|^2\leq C_2\int_{A_R}|\nabla u|^2=C_2\bigl(E(2R)-E(R)\bigr).
$$

Moving the $E(R)$ term to the left is the [hole-filling argument](../../../partial-differential-equation.md#hole-filling-argument):

$$
E(R)\leq\theta E(2R),\qquad\theta=\frac{C_2}{1+C_2}\in(0,1).
$$

Consequently $E(2^{-k}r_0)\leq\theta^kE(r_0)$. Put $\beta=-\log_2\theta>0$ and choose $\mu=\min\{\beta/2,1/2\}\in(0,1)$. For $2^{-k-1}r_0<r\leq2^{-k}r_0$, monotonicity gives

$$
E(r)\leq\theta^kE(r_0)\leq2^{-k\mu}E(r_0)\leq2^\mu(r/r_0)^\mu E(r_0).
$$

Dyadic endpoints can be assigned to either adjacent interval. Since $E(r_0)\leq\int_B|\nabla u|^2$, the requested [dyadic energy decay](../../../partial-differential-equation.md#dyadic-energy-decay) is

$$
\boxed{E(r)\leq K(r/r_0)^\mu\int_B|\nabla u|^2,\qquad K=2^\mu.}
$$

Both constants depend only on the dimension and [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) bounds, not on $u,x_0,r,r_0$.

There is a dimensional detail in the printed hint: an [annulus](../../../topology.md#annulus-mathematics) is disconnected in dimension one, so that [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) with a single average is false there. The conclusion still holds. In one dimension the weak equation gives $a(x)u'(x)=J$ almost everywhere for a [constant flux for a one-dimensional divergence-form equation](../../../elliptic-boundary-value-problem.md#constant-flux-for-a-one-dimensional-divergence-form-equation) $J$. Since $\lambda\leq a\leq\Lambda$,

$$
E(r)\leq\frac{2rJ^2}{\lambda^2},\qquad E(r_0)\geq\frac{2r_0J^2}{\Lambda^2},\qquad E(r)\leq(\Lambda/\lambda)^2(r/r_0)E(r_0).
$$

This implies the required estimate with, for example, $\mu=1/2$ and $K=(\Lambda/\lambda)^2$. If $J=0$, the estimate is immediate. Thus the proof also covers dimension one without using the inapplicable hint.

## 4

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

We use a [blow-up compactness proof of an interior Schauder estimate](../../../elliptic-boundary-value-problem.md#blow-up-compactness-proof-of-an-interior-schauder-estimate), with [Taylor normalization in elliptic blow-up arguments](../../../elliptic-boundary-value-problem.md#taylor-normalization-in-elliptic-blow-up-arguments). Fix $n,\mu,\delta$ and suppose no suitable constant exists. There would be solutions $u_j$ with forcing $f_j$ for which

$$
S_j^{\mathrm{in}}>\delta S_j+jN_j,\qquad S_j^{\mathrm{in}}=[D^2u_j]_{\mu;B_{1/2}},\quad S_j=[D^2u_j]_{\mu;B_1},\quad N_j=\|u_j\|_{C^2}+\|f_j\|_{C^{0,\mu}}.
$$

Choose distinct $x_j,y_j\in B_{1/2}$ such that, for $r_j=|y_j-x_j|$,

$$
A_j=\frac{|D^2u_j(y_j)-D^2u_j(x_j)|}{r_j^\mu}>\frac12S_j^{\mathrm{in}}.
$$

Then $S_j/A_j<2/\delta$, $N_j/A_j<2/j$, and

$$
r_j^\mu\leq\frac{2\|D^2u_j\|_\infty}{A_j}\leq\frac4j.
$$

In particular $r_j\to0$. Subtract the quadratic [Taylor polynomial](../../../calculus.md#taylor-polynomial) of $u_j$ at $x_j$ and rescale:

$$
v_j(z)=\frac{u_j(x_j+r_jz)-u_j(x_j)-r_j\nabla u_j(x_j)\cdot z-\tfrac12r_j^2z^TD^2u_j(x_j)z}{A_jr_j^{2+\mu}}.
$$

Its domain $\{z:x_j+r_jz\in B_1\}$ exhausts $\mathbb R^n$. The normalization gives

$$
v_j(0)=0,\quad\nabla v_j(0)=0,\quad D^2v_j(0)=0,\quad[D^2v_j]_{\mu}\leq2/\delta.
$$

[Taylor theorem](../../../calculus.md#taylor-theorem), or integration along line segments from zero, consequently bounds $D^2v_j,\nabla v_j,v_j$ on every fixed ball by constants times $|z|^\mu,|z|^{1+\mu},|z|^{2+\mu}$, respectively. The [Hessian matrices](../../../calculus.md#hessian-matrix) are [equicontinuous](../../../topological-analysis.md#equicontinuity). The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) and a diagonal subsequence therefore give $v_j\to v$ in $C^2$ on compact subsets of $\mathbb R^n$.

The rescaled equation is

$$
\Delta v_j(z)=\frac{f_j(x_j+r_jz)-f_j(x_j)}{A_jr_j^\mu},\qquad|\Delta v_j(z)|\leq\frac{[f_j]_\mu}{A_j}|z|^\mu\longrightarrow0
$$

on each compact set. Thus $v$ is harmonic and is smooth. Every entry of its [Hessian matrix](../../../calculus.md#hessian-matrix) is harmonic and has a global [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) at most $2/\delta$. The allowed [Liouville lemma for globally Hölder harmonic functions](../../../partial-differential-equation.md#liouville-lemma-for-globally-holder-harmonic-functions) makes each entry constant. Since $D^2v(0)=0$, all these constants are zero.

On the other hand, $e_j=(y_j-x_j)/r_j$ is a unit vector and $|D^2v_j(e_j)|=1$ by construction. A further subsequence has $e_j\to e$; the local $C^2$ convergence implies $|D^2v(e)|=1$, a contradiction. Hence the desired constant exists, and

$$
\boxed{[D^2u]_{\mu;B_{1/2}}\leq\delta[D^2u]_{\mu;B_1}+C(n,\mu,\delta)\bigl(\|u\|_{C^2(B_1)}+\|f\|_{C^{0,\mu}(B_1)}\bigr).}
$$

The global [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) on the limiting [Hessian matrix](../../../calculus.md#hessian-matrix), rather than a bound on its magnitude throughout space, is what makes this Liouville argument work.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

We prove [compactness of zero-boundary Poisson solutions](../../../elliptic-boundary-value-problem.md#compactness-of-zero-boundary-poisson-solutions). Here the printed $\partial\Omega$ must mean $\partial B_1$; otherwise the boundary condition refers to an unspecified set. Use this intended boundary condition throughout. Let $f=\Delta u$. A maximum-principle barrier gives a uniform bound on $u$: with $\psi(x)=(1-|x|^2)/(2n)$, we have $\Delta\psi=-1$ and $\psi=0$ on $\partial B_1$. Since $|f|\leq1$,

$$
\Delta(u-\psi)=f+1\geq0,\qquad\Delta(-u-\psi)=-f+1\geq0.
$$

The [weak maximum principle](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) gives $-\psi\leq u\leq\psi$, so $\|u\|_\infty\leq1/(2n)$.

Standard [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) on the smooth ball first gives $u\in C^{2,\mu}(\overline{B_1})$. The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) then gives

$$
\|u\|_{C^{2,\mu}(\overline{B_1})}\leq C\left(\|u\|_{C^0(\overline{B_1})}+\|f\|_{C^{0,\mu}(\overline{B_1})}\right)\leq C\left(1+\frac1{2n}\right).
$$

Thus the functions and all their derivatives through order two are uniformly bounded and [equicontinuous](../../../topological-analysis.md#equicontinuity) on the closed ball. The [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) gives a subsequence converging uniformly along with all these derivatives. Integration along line segments identifies the limiting derivatives, so the convergence is in $C^2(\overline{B_1})$.

It remains to keep the limit in the set, rather than merely proving [relative compactness](../../../topological-analysis.md#relatively-compact-subset). If $u_j\to u$ in $C^2$, then the zero boundary values pass to the limit and $f_j=\Delta u_j\to f=\Delta u$ uniformly. For each pair of distinct points,

$$
\frac{|f(x)-f(y)|}{|x-y|^\mu}=\lim_j\frac{|f_j(x)-f_j(y)|}{|x-y|^\mu}.
$$

Taking suprema gives $[f]_\mu\leq\liminf_j[f_j]_\mu$, while $\|f_j\|_\infty\to\|f\|_\infty$. Hence $\|f\|_{C^{0,\mu}}\leq1$. The limit belongs to the set, proving **[sequential compactness](../../../geometry-and-topology.md#sequentially-compact-space) in $C^2(\overline{B_1})$**. The fixed positive Hölder exponent supplies the compactness; a bound on the [supremum norm](../../../functional-analysis.md#supremum-norm) of $\Delta u$ alone would not supply this argument.

## 5

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient)

$$
b_n(y)=\frac2\pi\int_0^\pi u(x,y)\sin(nx)\,dx,\qquad n\geq1.
$$

They are continuous for $0\leq y\leq1$ and bounded by $2\|u\|_\infty$. On compact subintervals of $0<y<1$, the equation is [uniformly elliptic](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) with smooth coefficients. Local [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) at the flat vertical sides with zero boundary values permits differentiation and [integration by parts](../../../calculus.md#integration-by-parts) there. Thus

$$
y^2b_n''(y)=-\frac2\pi\int_0^\pi u_{xx}(x,y)\sin(nx)\,dx=n^2b_n(y).
$$

For completeness, this identity also follows in the distributional sense without assuming boundary derivatives initially. Integrate on $(\varepsilon,\pi-\varepsilon)$ against $\sin(nx)$ and a [test function](../../../distribution-theory.md#test-function) of $y$ with support away from zero and one. The [interior gradient estimate near a zero Dirichlet side](../../../distribution-theory.md#interior-gradient-estimate-near-a-zero-dirichlet-side) gives $|u_x|\leq C\varepsilon^{-1}\sup|u|$ on a nearby ball of radius comparable to $\varepsilon$; continuity and the zero side value make that supremum $o(1)$ uniformly over the support in $y$. Therefore the boundary products $u_x\sin(nx)$ and $u\cos(nx)$ tend to zero. Move the $y$ derivatives to the [test function](../../../distribution-theory.md#test-function) before taking $\varepsilon\downarrow0$. This proves the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation), which makes each $b_n$ smooth in $0<y<1$ and yields the same classical identity.

The [Cauchy-Euler differential equation](../../../differential-equation.md#cauchy-euler-equation) has [indicial roots](../../../differential-equation.md#indicial-root)

$$
p_n^\pm=\frac{1\pm\sqrt{1+4n^2}}2,\qquad b_n(y)=A_n y^{p_n^+}+B_n y^{p_n^-}.
$$

For $n\geq1$ the negative root is strictly negative. Boundedness as $y\downarrow0$ forces $B_n=0$. Continuity at $y=1$ identifies

$$
A_n=\frac2\pi\int_0^\pi u(x,1)\sin(nx)\,dx,\qquad |A_n|\leq2\|u\|_\infty.
$$

Because $p_n^+>n$, the series $\sum_{n\geq1}A_ny^{p_n^+}\sin(nx)$ converges absolutely and uniformly for $0\leq y\leq\rho<1$. On compact subsets with $y>0$, differentiated series converge as well. At each fixed $0<y<1$, its [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) equal those of $u(\cdot,y)$; completeness of the [Fourier sine basis](../../../fourier-series.md#fourier-sine-basis) in $L^2(0,\pi)$ and continuity in $x$ make the two functions equal. Therefore

$$
\boxed{u(x,y)=\sum_{n=1}^\infty A_ny^{(1+\sqrt{1+4n^2})/2}\sin(nx),\qquad (x,y)\in R.}
$$

This is also the requested sum over integers: take all coefficients with $n\leq0$ to be zero. Negative indices give redundant [Fourier modes](../../../fourier-analysis.md#fourier-mode), and the $n=0$ sine vanishes. No pointwise convergence of the ordinary [Fourier series](../../../fourier-series.md) on the top boundary is needed.

An important consequence is a [forced zero trace at a quadratically degenerate boundary](../../../elliptic-boundary-value-problem.md#forced-zero-trace-at-a-quadratically-degenerate-boundary). Indeed the absolute sum is bounded by $2\|u\|_\infty\sum_{n\geq1}y^n=2\|u\|_\infty y/(1-y)$ for $y<1$, which tends to zero as $y\downarrow0$, uniformly in $x$. Thus **$u(x,0)=0$** on the entire lower side. It follows also from $b_n(0)=0$ for every sine coefficient and completeness.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Choose continuous boundary values equal to $\sin x$ on the lower side and zero on the other three sides. These values agree at all four corners, so they define a continuous function on the boundary of the rectangle. Any solution would satisfy the zero vertical-side conditions of part (a), whose [Fourier sine series](../../../fourier-series.md#fourier-sine-series) forces its lower boundary trace to be zero. This contradicts the prescribed value $\sin x$ for $0<x<\pi$. Hence **these continuous [Dirichlet data](../../../differential-equation.md#dirichlet-boundary-data) admit no solution in $C^0(\overline R)\cap C^2(R)$**.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The missing hypothesis is **[uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) up to the boundary**. The principal coefficient matrix and its [quadratic form](../../../linear-algebra.md#quadratic-form) are

$$
a(x,y)=\begin{pmatrix}1&0\\0&y^2\end{pmatrix},\qquad a^{ij}\xi_i\xi_j=\xi_1^2+y^2\xi_2^2.
$$

Although this is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) at every interior point, no single positive [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) constant works on $R$: taking $\xi=(0,1)$ requires $y^2\geq\lambda$ for arbitrarily small positive $y$. The normal second-derivative coefficient vanishes on the lower side. This [degenerate ellipticity](../../../elliptic-boundary-value-problem.md#degenerate-elliptic-operator) allows the equation and boundedness to force a boundary trace, instead of allowing arbitrary continuous [Dirichlet data](../../../differential-equation.md#dirichlet-boundary-data). The coefficient matrix is [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form) at every interior point, but lacks the uniform lower bound used by the usual bounded-domain existence theorem.

## 6

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

With only $u\in L^2(\Omega)$ available, use a [distributional weak solution](../../../partial-differential-equation.md#weak-solution): for every [test function](../../../distribution-theory.md#test-function) $\eta\in C_c^\infty(\Omega)$ require

$$
\boxed{\int_\Omega u\,\Delta\eta=-\sum_{i=1}^n\int_\Omega b^iu\,D_i\eta+\int_\Omega(cu+f)\eta.}
$$

All terms are meaningful because the smooth coefficients are bounded on the compact support of the [test function](../../../distribution-theory.md#test-function) and $u$ is locally integrable. This is exactly $\Delta u=\sum_iD_i(b^iu)+cu+f$ as an identity of [distributions](../../../distribution-theory.md#distribution-mathematical-analysis). No first [weak derivative](../../../distribution-theory.md#weak-derivative) of $u$ is assumed in this definition, and no boundary condition is being imposed.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Fix $x$ with $\operatorname{dist}(x,\partial\Omega)>\sigma$ and use $\eta_x(y)=\phi_\sigma(x-y)$ as the [test function](../../../distribution-theory.md#test-function) in part (a). Its support lies compactly inside $\Omega$. Differentiating the [convolution](../../../fourier-analysis.md#convolution) under the integral is allowed, and $D_{y_i}\eta_x=-D_{x_i}\phi_\sigma(x-y)$ while $\Delta_y\eta_x=\Delta_x\phi_\sigma(x-y)$. Consequently

$$
\begin{aligned}
\Delta u_\sigma(x)&=\int_\Omega u(y)\Delta_y\eta_x(y)\,dy\\
&=-\sum_i\int_\Omega b^i(y)u(y)D_{y_i}\eta_x(y)\,dy+\int_\Omega(cu+f)(y)\eta_x(y)\,dy\\
&=\sum_iD_{x_i}\int_\Omega b^i(y)u(y)\phi_\sigma(x-y)\,dy+(cu)_\sigma(x)+f_\sigma(x).
\end{aligned}
$$

Thus

$$
\boxed{\Delta u_\sigma=\sum_iD_i(b^iu)_\sigma+(cu)_\sigma+f_\sigma}
$$

at every stated interior point. This is the [convolution derivative identity](../../../fourier-analysis.md#differentiation-commutes-with-convolution). The [convolutions](../../../fourier-analysis.md#convolution) are local, so no integrability of the smooth coefficients all the way to the boundary is needed. In particular, $(b^iu)_\sigma$ is the [convolution](../../../fourier-analysis.md#convolution) of the product; it must not be replaced by $b^iu_\sigma$ for a variable coefficient.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Choose nested interior open sets $U\subset\subset V\subset\subset W\subset\subset\Omega$. For small $\sigma$, part (b) gives a smooth equation on $V$ of the form

$$
\Delta u_\sigma=\operatorname{div}F_\sigma+G_\sigma,\qquad F_\sigma=(bu)_\sigma,\quad G_\sigma=(cu)_\sigma+f_\sigma.
$$

The [divergence-forcing interior H1 estimate](../../../distribution-theory.md#divergence-forcing-interior-h1-estimate) is

$$
\|u_\sigma\|_{H^1(U)}\leq C\left(\|u_\sigma\|_{L^2(V)}+\|F_\sigma\|_{L^2(V)}+\|G_\sigma\|_{L^2(V)}\right).
$$

One can obtain this estimate directly by testing the smooth equation against $\eta^2u_\sigma$ and applying [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products), with a [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one on $U$ and supported in $V$. The [approximate identity](../../../fourier-analysis.md#approximate-identity) and the $L^2$ [convolution](../../../fourier-analysis.md#convolution) bound give, uniformly in $\sigma$,

$$
\|u_\sigma\|_{L^2(V)}\leq\|u\|_{L^2(W)},\quad\|(bu)_\sigma\|_{L^2(V)}\leq\|b\|_{L^\infty(W)}\|u\|_{L^2(W)},
$$

with analogous bounds for $(cu)_\sigma$ and $f_\sigma$. The coefficients need only be bounded on $W$. Therefore $u_\sigma$ is bounded in $H^1(U)$. It converges to $u$ in $L^2(U)$, and [weak sequential compactness in a Hilbert space](../../../functional-analysis.md#weak-sequential-compactness-in-a-hilbert-space) in this [Sobolev space](../../../sobolev-space.md) gives $u\in H^1(U)$. Since $U$ was arbitrary, $u\in H^1_{\mathrm{loc}}(\Omega)$.

Now expand the [distributional derivative](../../../distribution-theory.md#distributional-derivative):

$$
\Delta u=b\cdot\nabla u+(\operatorname{div}b+c)u+f.
$$

Its right side belongs to $L^2_{\mathrm{loc}}$, so the interior $H^2$ [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) estimate gives $u\in H^2_{\mathrm{loc}}$. More generally, if $u\in H^m_{\mathrm{loc}}$ for an integer $m\geq1$, multiplication by the smooth coefficients puts the right side in $H^{m-1}_{\mathrm{loc}}$. Interior [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) then gives $u\in H^{m+1}_{\mathrm{loc}}$. This [elliptic regularity bootstrap](../../../distribution-theory.md#elliptic-regularity-bootstrap-with-smooth-lower-order-coefficients) proves $u\in H^k_{\mathrm{loc}}$ for every integer $k$.

For any nonnegative integer $\ell$, choose $k>\ell+n/2$. The [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) on compact interior subsets gives $u\in C^\ell_{\mathrm{loc}}$. Taking all $\ell$ proves **$u\in C^\infty(\Omega)$**, for its smooth representative. The first gain from $L^2$ to $H^1$ is the step supplied by the mollified equation; assuming $H^1$ in the initial definition would miss that step.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
