# Paper 107

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_107.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_107.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
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

## 1

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Assume real bounded coefficients, with a principal part defining a [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator), say $a^{ij}\xi_i\xi_j\geq\lambda|\xi|^2$ for some $\lambda>0$, and assume $c\leq0$. No smoothness of the boundary is needed for this classical [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators). Its conclusion is

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}.}
$$

If $c=0$, the zero may be omitted. Only the symmetric part of the principal coefficients contributes to the [Hessian matrix](../../../calculus.md#hessian-matrix) contraction.

For a strict inequality $Lu>0$, a positive interior maximum is impossible: there $Du=0$, $D^2u$ is negative semidefinite, and $cu\leq0$, so $Lu\leq0$. To reduce the non-strict case to this one, let $q(x)=e^{\kappa x_1}$. Boundedness of $b^1,c$ permits choosing $\kappa$ so large that

$$
Lq=q\bigl(\kappa^2a^{11}+\kappa b^1+c\bigr)
\geq q\bigl(\lambda\kappa^2-\|b^1\|_\infty\kappa-\|c\|_\infty\bigr)>0.
$$

Thus $L(u+\varepsilon q)>0$. The preceding maximum argument and continuity on the compact closure give

$$
\sup_\Omega(u+\varepsilon q)\leq\max\{0,\sup_{\partial\Omega}(u+\varepsilon q)\}.
$$

Let $\varepsilon\downarrow0$; the exponential is bounded on the bounded domain. This is the [exponential perturbation proof of the weak maximum principle with drift](../../../elliptic-boundary-value-problem.md#exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift), with the zeroth-order term included. For $c=0$, any interior maximum, of either sign, is impossible for the perturbed function, giving the sharper boundary bound. The sign restriction on $c$ is essential: a positive first [Dirichlet Laplacian eigenfunction](../../../partial-differential-equation.md#dirichlet-laplacian-eigenfunction) violates the conclusion for $L=\Delta+\lambda_1$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Apply the [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) to $q=|Dw|^2$. The [product rule](../../../calculus.md#product-rule) and the equation for the [harmonic function](../../../partial-differential-equation.md#harmonic-function) give

$$
\Delta q=2\sum_{i,j}(D_{ij}w)^2+2\sum_iD_iw\,D_i\Delta w
=2|D^2w|^2\geq0.
$$

The function $q$ is twice differentiable inside and continuous on the closure, by the prescribed regularity. Hence $\sup_\Omega q\leq\sup_{\partial\Omega}q$. Conversely, each boundary value of $q$ is a limit of values at interior points, so the reverse inequality holds for the suprema. Taking square roots proves the [gradient maximum principle for harmonic functions](../../../partial-differential-equation.md#gradient-maximum-principle-for-harmonic-functions):

$$
\boxed{\sup_\Omega|Dw|=\sup_{\partial\Omega}|Dw|.}
$$

This argument controls the length of the entire [gradient](../../../calculus.md#gradient), without comparing its separate components.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

By continuity on the compact closure, $v$ has a maximum and minimum. If its maximum were greater than one, the boundary hypothesis would force that maximum to occur at an interior point $x_0$. There $\Delta v(x_0)\leq0$, whereas

$$
v(x_0)^3-v(x_0)=v(x_0)\bigl(v(x_0)^2-1\bigr)>0,
$$

a contradiction. If its minimum were less than minus one, it would again be interior, where $\Delta v\geq0$ but $v^3-v<0$. Therefore

$$
\boxed{-1\leq v\leq1\quad\text{on }\overline\Omega,\qquad \sup_\Omega|v|\leq1.}
$$

This is a direct maximum/minimum argument for a [nonlinear elliptic boundary value problem](../../../elliptic-boundary-value-problem.md#nonlinear-elliptic-boundary-value-problem); treating its nonlinearity as a zeroth-order coefficient of fixed nonpositive sign would not be justified.

## 2

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume an [interior sphere condition](../../../elliptic-boundary-value-problem.md#interior-sphere-condition) at $y$, and assume the coefficients are bounded and the principal part defines a [uniformly elliptic operator](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) near its tangent [Euclidean ball](../../../functional-analysis.md#euclidean-ball). Shrinking the [Euclidean ball](../../../functional-analysis.md#euclidean-ball) while keeping it tangent if necessary, arrange that $\overline{B_R(z)}\setminus\{y\}\subset\Omega$. Write $\nu=(y-z)/R$, the outward radial direction. The conclusion of the [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma) in the regularity stated in the question is

$$
\boxed{\liminf_{t\downarrow0}\frac{u(y)-u(y-t\nu)}{t}>0.}
$$

If the one-sided [normal derivative](../../../differential-geometry.md#normal-derivative) exists, this says $\partial_\nu u(y)>0$. For a $C^1$ boundary its outward normal agrees with the tangent [Euclidean ball](../../../functional-analysis.md#euclidean-ball)'s radial normal. Continuity alone does not guarantee that the derivative exists, so its existence must be added when asserting a finite derivative.

On the annulus $R/2<r=|x-z|<R$, use the barrier

$$
h(x)=e^{-kr^2}-e^{-kR^2}>0.
$$

The operator has no zeroth-order term, and differentiation gives

$$
Lh=e^{-kr^2}\left(4k^2a^{ij}(x_i-z_i)(x_j-z_j)-2k\operatorname{tr}a-2kb^i(x_i-z_i)\right)>0
$$

for sufficiently large $k$: the quadratic-in-$k$ term is at least $k^2\lambda R^2$, while the remaining terms are bounded multiples of $k$.

On the inner sphere, compactness and strict inequality give a positive minimum of $u(y)-u(x)$. Choose $\varepsilon>0$ small enough that $u-u(y)+\varepsilon h\leq0$ there. The same inequality holds on the outer sphere since $h=0$. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) yields $u-u(y)+\varepsilon h\leq0$ throughout the annulus. Along the inward radius,

$$
\frac{u(y)-u(y-t\nu)}{t}\geq\varepsilon\frac{e^{-k(R-t)^2}-e^{-kR^2}}{t}
\longrightarrow2\varepsilon kRe^{-kR^2}>0.
$$

This proves the lemma. The [interior sphere condition](../../../elliptic-boundary-value-problem.md#interior-sphere-condition) supplies precisely the geometry needed for the barrier; no global boundary regularity is used.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Here a domain is connected. Suppose both a negative point and a zero point exist. The open set $D=\{v<0\}$ then has a boundary point $q$ inside $\Omega$. Choose $z\in D$ close enough to $q$ that the [Euclidean ball](../../../functional-analysis.md#euclidean-ball) of radius $R=\operatorname{dist}(z,Z)$ stays compactly inside $\Omega$; it is contained in $D$ and touches $Z$ at some $y$. Attainment of this distance follows by restricting to a compact neighbourhood of $q$.

On that [Euclidean ball](../../../functional-analysis.md#euclidean-ball) $v$ is twice differentiable and

$$
\Delta v=-v>0,\qquad v(y)=0>v(x)\quad(x\in B_R(z)).
$$

The [Hopf boundary point lemma](../../../elliptic-boundary-value-problem.md#hopf-lemma) gives a strictly positive outward radial derivative at $y$. But $y$ is an interior maximum of the $C^1$ function $v$ on $\Omega$, so $Dv(y)=0$. This contradiction proves the [Hopf dichotomy with classical regularity away from the zero set](../../../elliptic-boundary-value-problem.md#hopf-dichotomy-with-classical-regularity-away-from-the-zero-set):

$$
\boxed{v\equiv0\quad\text{or}\quad v<0\text{ throughout }\Omega.}
$$

For the requested weaker-regularity counterexample take $\Omega=(-1,1)^n$ and

$$
\boxed{v(x)=-\max\{\sin x_1,0\}.}
$$

It is a [locally Lipschitz function](../../../real-analysis.md#locally-lipschitz-function) and nonpositive. Its negative set is $x_1>0$, where $v=-\sin x_1$ is smooth and $\Delta v+v=0$. On $x_1\leq0$ it is zero. The [normal derivative](../../../differential-geometry.md#normal-derivative) jumps from zero to minus one across $x_1=0$, so it is not $C^1$. All other hypotheses hold; imposing the equation also across that interface would be an additional condition absent from the question.

## 3

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [global Schauder estimate](../../../elliptic-boundary-value-problem.md#global-schauder-estimate) on a bounded $C^{2,\alpha}$ domain is

$$
\boxed{\|u\|_{C^{2,\alpha}(\overline\Omega)}
\leq C\left(\|u\|_{C^0(\overline\Omega)}+\|f\|_{C^{0,\alpha}(\overline\Omega)}
+\|\psi\|_{C^{2,\alpha}(\overline\Omega)}\right).}
$$

Here $C$ depends on $n,\alpha$, the domain's boundary regularity and $\|c\|_{C^{0,\alpha}}$, but not on the particular solution or data. The $C^0$ term is needed before uniqueness has been established. The given $\psi$ is an extension of the boundary data to the closure.

For $c\leq0$, choose $d$ with $\Omega\subset\{|x_1|<d\}$ and set $M=\sup_{\partial\Omega}|\psi|$, $F=\sup_\Omega|f|$. The hinted function

$$
b(x)=M+(e^{2d}-e^{x_1+d})F
$$

is nonnegative, dominates $|\psi|$ on the boundary, and satisfies

$$
(\Delta+c)b=-e^{x_1+d}F+cb\leq-F,
$$

since $x_1+d>0$. Therefore $(\Delta+c)(u-b)=f-(\Delta+c)b\geq0$ and $(\Delta+c)(-u-b)=-f-(\Delta+c)b\geq0$. Both functions are nonpositive on the boundary. The [weak maximum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) gives $|u|\leq b$, hence the [supremum norm barrier for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#supremum-norm-barrier-for-an-elliptic-dirichlet-problem):

$$
\boxed{\|u\|_\infty\leq M+e^{2d}F.}
$$

Unlike the full [Schauder estimate](../../../elliptic-boundary-value-problem.md#schauder-estimates), this last constant depends only on a slab containing $\Omega$, and is independent of how negative $c$ is.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $L=\Delta+c$ with real $c$, and let

$$
N=\{z\in C^{2,\alpha}(\overline\Omega):Lz=0,\ z|_{\partial\Omega}=0\}.
$$

The [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem) says that $N$ is finite-dimensional. If $N=0$, all the prescribed data admit a unique solution. In general the exact [boundary compatibility in the self-adjoint Fredholm alternative](../../../elliptic-boundary-value-problem.md#boundary-compatibility-in-the-self-adjoint-fredholm-alternative) is

$$
\boxed{\int_\Omega fz\,dx+\int_{\partial\Omega}\psi\,\partial_\nu z\,dS=0
\quad\text{for every }z\in N.}
$$

These conditions are necessary and sufficient; when they hold, all solutions form $u_0+N$. Thus in the second branch some data are incompatible, while compatible data have nonunique solutions. The outward [normal derivative](../../../differential-geometry.md#normal-derivative) fixes the displayed sign.

To prove the alternative, put $X=\{w\in C^{2,\alpha}(\overline\Omega):w|_{\partial\Omega}=0\}$ and $Y=C^{0,\alpha}(\overline\Omega)$. The standard zero-boundary [Poisson equation](../../../partial-differential-equation.md#poisson-equation) theorem makes $\Delta:X\to Y$ an isomorphism. Multiplication by $c$, followed by $\Delta^{-1}$, is a [compact operator](../../../compact-operator.md) $K:X\to X$: the embedding $C^{2,\alpha}\hookrightarrow C^{0,\alpha}$ is compact, and multiplication is bounded. Writing $u=\psi+w$ gives

$$
(I+K)w=\Delta^{-1}F,\qquad F=f-\Delta\psi-c\psi.
$$

The [Fredholm alternative for a compact operator](../../../compact-operator.md#fredholm-alternative) implies finite kernel and cokernel of equal dimension, and invertibility exactly when the kernel vanishes.

For the explicit compatibility conditions, use the [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) Dirichlet realization of $L$ on $L^2$. It has compact resolvent: a sufficiently large positive shift of $-L$ is [coercive](../../../linear-algebra.md#coercive-bilinear-form), its inverse gains two derivatives, and the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) makes that inverse compact. The [Fredholm solvability condition for a self-adjoint operator](../../../linear-operator-theory.md#fredholm-solvability-condition-for-a-self-adjoint-operator) is $F\perp N$. Standard boundary [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) upgrades the resulting [weak solution](../../../partial-differential-equation.md#weak-solution) to $C^{2,\alpha}$ for these data and boundary. Thus it gives the same kernel and solvability as the preceding Hölder-space formulation.

Finally [Green second identity](../../../partial-differential-equation.md#green-second-identity), with $z=0$ on the boundary and $Lz=0$, gives

$$
\int_\Omega zL\psi\,dx=-\int_{\partial\Omega}\psi\partial_\nu z\,dS.
$$

Consequently $\int zF=\int zf+\int\psi\partial_\nu z$, proving both necessity and sufficiency with the stated sign. If using complex data and real $c$, replace $z$ by $\overline z$ in the pairings.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the [supremum norm barrier for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#supremum-norm-barrier-for-an-elliptic-dirichlet-problem) to obtain a domain-only constant $C_\Omega=e^{2d}$. Split the coefficient as $c=c_-+c_+$, where $c_-\leq0$ and $c_+=\max(c,0)$. Both parts are [Hölder continuous functions](../../../sobolev-space.md#holder-condition). Choose

$$
\boxed{\epsilon(\Omega)=\frac1{2C_\Omega}>0.}
$$

If $u$ solves the homogeneous zero-boundary problem for $\Delta+c$, then

$$
(\Delta+c_-)u=-c_+u.
$$

Part (a), applied to this nonpositive zeroth-order coefficient, gives

$$
\|u\|_\infty\leq C_\Omega\|c_+u\|_\infty
\leq C_\Omega\epsilon\|u\|_\infty=\tfrac12\|u\|_\infty.
$$

Hence $u=0$. The [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem) now gives existence and uniqueness for every forcing and boundary datum in the stated [Hölder spaces](../../../sobolev-space.md#holder-space). This proves the [small positive zeroth-order perturbation of a Dirichlet problem](../../../elliptic-boundary-value-problem.md#small-positive-zeroth-order-perturbation-of-a-dirichlet-problem) without imposing a bound on the negative part of $c$. The value of $\epsilon$ need not be optimal.

## 4

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use the paper's classical norm convention: $|u|_{2;U}$ is the [derivative supremum norm](../../../functional-analysis.md#derivative-supremum-norm) through order two, not an $L^2$ norm. Write $H(u;U)=[D^2u]_{\alpha;U}$ and $Q(u,f)=|u|_{2;B_1}+|f|_{0,\alpha;B_1}$, where the latter is the full [Hölder norm](../../../sobolev-space.md#holder-norm) of the forcing.

Fix $0<\delta<1$. If the asserted estimate failed, rescaling the functions by their global [Hessian matrix](../../../calculus.md#hessian-matrix) [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) would produce $u_j,f_j$ with

$$
H(u_j;B_1)=1,\qquad H(u_j;B_{1/2})>\delta+jQ(u_j,f_j).
$$

In particular $Q(u_j,f_j)\to0$. Choose $x_j,y_j\in B_{1/2}$ for which

$$
|D^2u_j(y_j)-D^2u_j(x_j)|>\tfrac\delta2|y_j-x_j|^\alpha.
$$

The [supremum norm](../../../functional-analysis.md#supremum-norm) of $D^2u_j$ tends to zero, so $r_j=|y_j-x_j|\to0$. Let $P_j$ be the quadratic [Taylor polynomial](../../../calculus.md#taylor-polynomial) of $u_j$ at $x_j$, and define

$$
U_j(z)=\frac{u_j(x_j+r_jz)-P_j(x_j+r_jz)}{r_j^{2+\alpha}}.
$$

The domains contain $B_{1/(2r_j)}$, and $U_j,DU_j,D^2U_j$ vanish at zero. Moreover

$$
[D^2U_j]_{\alpha}\leq1,\qquad
\Delta U_j(z)=r_j^{-\alpha}\bigl(f_j(x_j+r_jz)-f_j(x_j)\bigr).
$$

The right side is bounded by $[f_j]_\alpha|z|^\alpha$ and tends to zero locally uniformly. The normalized [Hessian matrix](../../../calculus.md#hessian-matrix) bound controls $|D^2U_j(z)|\leq|z|^\alpha$; integration along line segments then bounds $DU_j,U_j$ on every compact [Euclidean ball](../../../functional-analysis.md#euclidean-ball). [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) and a [diagonal subsequence argument](../../../real-analysis.md#diagonal-subsequence-argument) give convergence in $C^2$ on compact subsets to an entire [harmonic function](../../../partial-differential-equation.md#harmonic-function) $U$, with $[D^2U]_{\alpha;\mathbb R^n}\leq1$ and $D^2U(0)=0$.

After a further subsequence $z_j=(y_j-x_j)/r_j\to z_*$ with $|z_*|=1$. The normalization ensures $|D^2U(z_*)|\geq\delta/2$. But each second derivative of $U$ is harmonic and has finite global [Hölder seminorm](../../../sobolev-space.md#holder-seminorm) with exponent below one. The supplied Liouville theorem makes each derivative constant; it is the globally Hölder case of the [polynomial-growth Liouville theorem for harmonic functions](../../../partial-differential-equation.md#polynomial-growth-liouville-theorem-for-harmonic-functions). Its value at zero makes it zero, a contradiction. This [blow-up compactness proof of an interior Schauder estimate](../../../elliptic-boundary-value-problem.md#blow-up-compactness-proof-of-an-interior-schauder-estimate) establishes

$$
\boxed{H(u;B_{1/2})\leq\delta H(u;B_1)+C_{n,\alpha,\delta}Q(u,f).}
$$

To absorb the term on the larger [Euclidean ball](../../../functional-analysis.md#euclidean-ball), rescale this estimate to [Euclidean balls](../../../functional-analysis.md#euclidean-ball) contained in $B_s$. For $1/2\leq r<s<1$, pairs separated by less than $(s-r)/2$ are controlled in a [Euclidean ball](../../../functional-analysis.md#euclidean-ball) centred at their first point; farther pairs are controlled directly by $\|D^2u\|_\infty$. Thus

$$
H(u;B_r)\leq\delta H(u;B_s)+C_\delta(s-r)^{-2-\alpha}Q(u,f).
$$

This is the covering step in the [Simon absorption lemma](../../../elliptic-boundary-value-problem.md#simon-absorption-lemma). Take $r_j=1-2^{-j-1}$ and fix $\delta<2^{-2-\alpha}$. Iterating makes the remainder $\delta^jH(u;B_{r_j})$ tend to zero, since the global seminorm is finite; the error terms form a convergent geometric series. Consequently

$$
\boxed{[D^2u]_{\alpha;B_{1/2}}\leq C_{n,\alpha}\bigl(|u|_{2;B_1}+|f|_{0,\alpha;B_1}\bigr).}
$$

For the requested failure of the weaker estimate, take $u_m=m^{-2}\sin(mx_1)$ and $f_m=-\sin(mx_1)$. The [derivative supremum norm](../../../functional-analysis.md#derivative-supremum-norm) $|u_m|_2$ and $\|f_m\|_\infty$ remain bounded, but comparison at $0$ and $\pi e_1/(2m)$, both in $B_{1/2}$ for large $m$, gives

$$
\boxed{[D^2u_m]_{\alpha;B_{1/2}}\geq(2m/\pi)^\alpha\longrightarrow\infty.}
$$

This proves the [necessity of Hölder forcing for Schauder estimates](../../../elliptic-boundary-value-problem.md#necessity-of-holder-forcing-for-schauder-estimates). Every member of the sequence is smooth; failure comes from the increasing frequency, not from any lack of individual regularity.

## 5

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Adopt the sign convention that a [weak supersolution](../../../elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation) for $Lu=D_i(a^{ij}D_ju)$ satisfies $Lu\leq0$, or $\int a^{ij}D_juD_i\varphi\geq0$ for every nonnegative compactly supported [test function](../../../distribution-theory.md#test-function). For a nonnegative supersolution, the [Weak Harnack inequality](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality) gives some $q>0$ and $C_H\geq1$, depending only on $n,\lambda,\Lambda$, such that

$$
\boxed{\left(\frac1{|B_{1/2}|}\int_{B_{1/2}}u^q\,dx\right)^{1/q}
\leq C_H\operatorname*{ess\,inf}_{B_{1/2}}u.}
$$

Here $|E|^{-1}\int_E$ denotes the average over $E$; equivalently the right side gives a lower bound for the [essential infimum](../../../real-analysis.md#essential-infimum). One may take a sufficiently small positive exponent, so no assumption $q\geq1$ is needed. The inequality is unchanged under translations and dilations of the [Euclidean balls](../../../functional-analysis.md#euclidean-ball).

Since a [Sobolev space](../../../sobolev-space.md) element is defined up to changes on a null set, the infimum is initially essential. After choosing a continuous representative it is the ordinary infimum. Without choosing such a representative, an arbitrary pointwise infimum cannot be bounded by an integral.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Work first with essential bounds. On a [Euclidean ball](../../../functional-analysis.md#euclidean-ball) $B_R(x_0)\Subset B_1$, put $M=\operatorname*{ess\,sup}_{B_R}u$, $m=\operatorname*{ess\,inf}_{B_R}u$ and $\omega=M-m$. The functions $M-u$ and $u-m$ are nonnegative [weak solutions](../../../partial-differential-equation.md#weak-solution), hence [weak supersolutions](../../../elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation). In $B_{R/2}$, at least one of the sets $\{u\leq(M+m)/2\}$ and $\{u\geq(M+m)/2\}$ has at least half the measure.

In the first case, the [Weak Harnack inequality](../../../elliptic-boundary-value-problem.md#weak-harnack-inequality) applied to $M-u$ gives

$$
C_H\bigl(M-\operatorname*{ess\,sup}_{B_{R/2}}u\bigr)
\geq\left(\frac1{|B_{R/2}|}\int_{B_{R/2}}(M-u)^q\right)^{1/q}
\geq2^{-1-1/q}\omega.
$$

In the second case, applying it to $u-m$ gives the same lower bound for the improvement of the minimum. Thus the [oscillation decay estimate](../../../elliptic-boundary-value-problem.md#oscillation-decay-estimate) is

$$
\boxed{\operatorname{osc}_{B_{R/2}}u\leq\tau\operatorname{osc}_{B_R}u,
\qquad \tau=1-C_H^{-1}2^{-1-1/q}\in(0,1).}
$$

This measure argument works even when $q<1$, avoiding a false use of the triangle inequality in that range.

Iteration yields $\operatorname{osc}_{B_r(x_0)}u\leq C(r/R)^\mu\operatorname{osc}_{B_R(x_0)}u$, with, for example, $\mu=\min\{1/2,-\log\tau/\log2\}\in(0,1)$. At [Lebesgue points](../../../measure-theory.md#lebesgue-point) the shrinking oscillations define a unique continuous representative, and the estimate extends to every point by continuity. For $x,y\in B_{1/4}$ at distance less than $1/4$, apply the estimate to a [Euclidean ball](../../../functional-analysis.md#euclidean-ball) centred at $x$ with initial radius $1/2$ and final radius comparable to $|x-y|$. This [Euclidean ball](../../../functional-analysis.md#euclidean-ball) stays in $B_1$. Larger distances use the trivial bound $2\|u\|_\infty$. We obtain

$$
\boxed{[u]_{C^{0,\mu}(\overline{B_{1/4}})}\leq C\|u\|_{L^\infty(B_1)},
\qquad u\in C^{0,\mu}(\overline{B_{1/4}}).}
$$

The constants depend only on $n,\lambda,\Lambda$. This derives the relevant conclusion of the [De Giorgi-Nash-Moser theorem](../../../elliptic-boundary-value-problem.md#de-giorgi-nash-moser-theorem) directly from part (a).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

First prove the hinted [Caccioppoli inequality](../../../partial-differential-equation.md#caccioppoli-inequality). Testing the [weak formulation](../../../partial-differential-equation.md#weak-formulation) with $u_k\varphi^2$ is legitimate by approximation in the zero-boundary [Sobolev space](../../../sobolev-space.md). Let $\Lambda_*=\operatorname*{ess\,sup}\|a(x)\|_{\mathrm{op}}\leq n\Lambda$. Then

$$
\lambda\int|Du_k|^2\varphi^2
\leq2\Lambda_*\int|u_k|\,|Du_k|\,|\varphi|\,|D\varphi|
\leq\tfrac\lambda2\int|Du_k|^2\varphi^2
+\frac{2\Lambda_*^2}{\lambda}\int u_k^2|D\varphi|^2,
$$

by [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products). Hence

$$
\boxed{\int|Du_k|^2\varphi^2\leq\frac{4\Lambda_*^2}{\lambda^2}\int u_k^2|D\varphi|^2.}
$$

No derivative of the measurable coefficient [matrix](../../../vector-space.md#matrix) is taken.

Set $w_k=u_k/\sup_{B_1}|u_k|$. The denominator is finite and positive because $u_k$ is continuous on the compact closure and nonzero. Each $w_k$ solves the same linear equation and $|w_k|\leq1$. For every $\theta<1$, choose a [cutoff function](../../../distribution-theory.md#cutoff-function) equal to one on $B_\theta$ and supported in a slightly larger interior [Euclidean ball](../../../functional-analysis.md#euclidean-ball). The energy bound gives a uniform $W^{1,2}(B_\theta)$ bound.

Take radii $\theta_j\uparrow1$. Weak compactness and a [diagonal subsequence argument](../../../real-analysis.md#diagonal-subsequence-argument) produce one subsequence converging weakly in $W^{1,2}(B_{\theta_j})$ for every $j$, with consistent restrictions defining $v\in W^{1,2}_{\mathrm{loc}}(B_1)$. Part (b) and the [Arzelà-Ascoli theorem](../../../topological-analysis.md#arzela-ascoli-theorem) allow a further subsequence converging uniformly on $\overline{B_{1/4}}$. Its uniform limit agrees almost everywhere with the weak limit and supplies its continuous representative there.

For every smooth compactly supported [test function](../../../distribution-theory.md#test-function), choose $j$ containing its support. Since $a^{ij}D_i\varphi\in L^2$ and $Dw_k$ converges weakly there,

$$
\int a^{ij}D_jvD_i\varphi
=\lim_k\int a^{ij}D_jw_kD_i\varphi=0.
$$

Thus the [compactness of normalized weak elliptic solutions](../../../elliptic-boundary-value-problem.md#compactness-of-normalized-weak-elliptic-solutions) gives

$$
\boxed{w_{k'}\longrightarrow v\text{ uniformly on }\overline{B_{1/4}},\qquad
Lv=0\text{ weakly in every }B_\theta,\ 0<\theta<1.}
$$

The diagonal step is needed to retain the equation beyond the small [Euclidean ball](../../../functional-analysis.md#euclidean-ball) of [uniform convergence](../../../real-analysis.md#uniform-convergence). The limit need not be nonzero: for the [Laplacian](../../../calculus.md#laplacian) in dimension at least two, the normalized [harmonic functions](../../../partial-differential-equation.md#harmonic-function) $\operatorname{Re}(x_1+ix_2)^k$ tend uniformly to zero on each smaller [Euclidean ball](../../../functional-analysis.md#euclidean-ball).

## 6

↑ **Parent:** [Paper 107](paper-107.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For the [divergence-form elliptic operator](../../../elliptic-boundary-value-problem.md#divergence-form-elliptic-operator) use the [weak subsolution](../../../elliptic-boundary-value-problem.md#weak-subsolution-of-a-divergence-form-elliptic-equation) convention $\int a^{ij}D_juD_i\varphi\leq0$ for nonnegative [test functions](../../../distribution-theory.md#test-function). Set $u_\varepsilon=u+\varepsilon$ and test with $\varphi=\eta^2u_\varepsilon^{\beta-1}$, where $\beta>1$. The [Sobolev chain rule](../../../distribution-theory.md#sobolev-chain-rule) makes this test admissible; boundedness and the positive regularization control the derivative of its power. Ellipticity and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give, with $X=\int|Du|^2u_\varepsilon^{\beta-2}\eta^2$ and $Y=\int u_\varepsilon^\beta|D\eta|^2$,

$$
\lambda(\beta-1)X\leq2\Lambda_*X^{1/2}Y^{1/2},\qquad
\Lambda_*\geq\operatorname*{ess\,sup}\|a(x)\|_{\mathrm{op}}.
$$

Division when $X>0$, and the trivial case $X=0$, establish the [power Caccioppoli inequality](../../../partial-differential-equation.md#power-caccioppoli-inequality). Letting $\varepsilon\downarrow0$ gives

$$
\boxed{\int|Du|^2u^{\beta-2}\eta^2\leq
\frac{4\Lambda_*^2}{\lambda^2(\beta-1)^2}\int u^\beta|D\eta|^2.}
$$

For $1<\beta<2$ this limit uses the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma); the [gradient of a Sobolev function vanishes on a level set](../../../distribution-theory.md#gradient-of-a-sobolev-function-vanishes-on-a-level-set), so the weighted integrand is assigned zero on $\{u=0\}$. The same regularization justifies differentiating $u^{\beta/2}\eta$ in $W^{1,2}$.

The PDF bounds individual entries by $\Lambda$. Then $\Lambda_*\leq n\Lambda$: dimensional factors are included in the ellipticity constants when the first estimate is written as $C(\lambda,\Lambda)$. With literal entrywise bounds, the explicit valid constant displayed here is $4n^2\Lambda^2/\lambda^2$. If $\Lambda$ bounds the [operator norm](../../../continuous-dual-space.md#operator-norm) instead, it is $4\Lambda^2/\lambda^2$. This distinction does not alter any later conclusion, whose constants explicitly depend on $n$.

For $n\geq3$, put $\sigma=n/(n-2)$. Apply the [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) to $g=u^{\beta/2}\eta$ and use

$$
\int|Dg|^2\leq\frac{\beta^2}{2}\int|Du|^2u^{\beta-2}\eta^2
+2\int u^\beta|D\eta|^2.
$$

For $\beta\geq p>1$, $\beta/(\beta-1)\leq p/(p-1)$, so the resulting constant is uniform in $\beta$. Taking a cutoff equal to one on $B_r$, supported in $B_R$, with $|D\eta|\leq C/(R-r)$, yields

$$
\boxed{\|u\|_{L^{\sigma\beta}(B_r)}
\leq C_p^{1/\beta}(R-r)^{-2/\beta}\|u\|_{L^\beta(B_R)},\qquad\beta\geq p.}
$$

At $R=1$ a compactly supported cutoff can still be chosen with this bound by leaving an outer margin; alternatively pass to the limit from smaller radii.

For [Moser iteration](../../../elliptic-boundary-value-problem.md#moser-iteration), set $\beta_j=p\sigma^j$ and $r_j=1/2+2^{-j-1}$. Repeated use of the preceding estimate bounds the successive norms by

$$
\|u\|_{L^p(B_1)}\prod_{j\geq0}C_p^{1/\beta_j}2^{(2j+4)/\beta_j}.
$$

This product is finite because

$$
\sum_{j\geq0}\frac1{\beta_j}=\frac n{2p},\qquad
\sum_{j\geq0}\frac j{\beta_j}=\frac{n(n-2)}{4p}.
$$

As the exponents tend to infinity, their norms on the [Euclidean ball](../../../functional-analysis.md#euclidean-ball) of radius $1/2$ tend to its [essential supremum](../../../measure-theory.md#essential-supremum). Therefore

$$
\boxed{\|u\|_{L^\infty(B_{1/2})}\leq C_{n,p,\lambda,\Lambda}\|u\|_{L^p(B_1)}.}
$$

The power $\beta$ is independent of the exponents of [Hölder continuity](../../../sobolev-space.md#holder-condition) in earlier questions.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For any $R>0$, set $U_R(y)=u(Ry)$ and $a_R^{ij}(y)=a^{ij}(Ry)$. These coefficients retain the same bounds and ellipticity, and a change of variables in the [weak formulation](../../../partial-differential-equation.md#weak-formulation) shows that $U_R$ is a nonnegative [weak subsolution](../../../elliptic-boundary-value-problem.md#weak-subsolution-of-a-divergence-form-elliptic-equation) on $B_1$. Part (a) gives the scale-correct estimate

$$
\boxed{\|u\|_{L^\infty(B_{R/2})}
\leq CR^{-n/p}\|u\|_{L^p(B_R)}
\leq CR^{-n/p}\|u\|_{L^p(\mathbb R^n)}.}
$$

The constant is independent of $R$. Fix a [Euclidean ball](../../../functional-analysis.md#euclidean-ball) $B_s$ and let $R\to\infty$ with $R>2s$. The right side tends to zero, so $u=0$ almost everywhere on $B_s$. Since $s$ is arbitrary, the [Liouville theorem for integrable nonnegative elliptic subsolutions](../../../elliptic-boundary-value-problem.md#liouville-theorem-for-integrable-nonnegative-elliptic-subsolutions) proves

$$
\boxed{u=0\text{ almost everywhere on }\mathbb R^n.}
$$

This is $u\equiv0$ as a [Sobolev space](../../../sobolev-space.md) element. Any continuous representative is identically zero pointwise; an arbitrary measurable representative can be modified at isolated points without changing the weak equation. Integrability and the explicit scaling force the conclusion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
