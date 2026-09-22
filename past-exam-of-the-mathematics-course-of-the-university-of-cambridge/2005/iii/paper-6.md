# Paper 6

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper6.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper6.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) states that in a complete [metric space](../../../topological-analysis.md#metric-space), a [countable](../../../set-theory.md#countable-set) intersection of open [dense](../../../topology.md#dense-set) sets is [dense](../../../topology.md#dense-set). Equivalently, a nonempty [complete metric space](../../../topological-analysis.md#complete-metric-space) cannot be a [countable union](../../../set.md#countable-union) of [nowhere dense sets](../../../topological-analysis.md#nowhere-dense-set), where a set is [nowhere dense](../../../topological-analysis.md#nowhere-dense-set) if its closure has empty interior.

Here is the proof. Let $G_1,G_2,\ldots$ be open [dense](../../../topology.md#dense-set) sets and let $U$ be any nonempty [open set](../../../topology.md#open-set). Choose a point $a_1\in U\cap G_1$ and a radius $0<r_1<1/2$ such that the [closed ball](../../../topological-analysis.md#closed-ball) $B_1=\overline B(a_1,r_1)$ lies inside $U\cap G_1$. Inductively choose $a_{m+1}$ in the nonempty [open set](../../../topology.md#open-set) $B(a_m,r_m)\cap G_{m+1}$, and then a radius $0<r_{m+1}<2^{-m-1}$ such that

$$
B_{m+1}=\overline B(a_{m+1},r_{m+1})\subseteq B(a_m,r_m)\cap G_{m+1}.
$$

Thus the [closed](../../../topology.md#closed-set) balls are nested and their radii tend to zero. For $j,k\geq m$, both centers lie in $B_m$, so $d(a_j,a_k)\leq2r_m$. They form a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence). [Completeness](../../../topological-analysis.md#completeness) gives a limit $a$, and closedness puts it in every $B_m$. Consequently $a\in U\cap\bigcap_mG_m$. As $U$ was arbitrary, **the intersection is [dense](../../../topology.md#dense-set)**.

To obtain the equivalent formulation, take complements of the closures of the [nowhere dense](../../../topological-analysis.md#nowhere-dense-set) sets; those complements are open [dense](../../../topology.md#dense-set). Conversely, complements of open [dense](../../../topology.md#dense-set) sets are [closed](../../../topology.md#closed-set) with empty interior. In particular, a [countable](../../../set-theory.md#countable-set) [closed](../../../topology.md#closed-set) cover of a nonempty [complete metric space](../../../topological-analysis.md#complete-metric-space) must contain a set with nonempty interior.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For each nonzero [integer](../../../number-theory.md#integer) tuple $k=(k_1,\ldots,k_{n+1})$, put

$$
H_k=\left\{x\in\mathbb R^n:\sum_{j=1}^nk_jx_j=k_{n+1}\right\}.
$$

If its first $n$ coordinates are all zero, then $k_{n+1}\ne0$ and $H_k$ is empty. Otherwise it is a [closed](../../../topology.md#closed-set) proper [affine hyperplane](../../../vector-space.md#affine-hyperplane). It has empty interior: from any of its points, an arbitrarily small displacement in the nonzero normal direction $(k_1,\ldots,k_n)$ leaves it. Thus every $H_k$ is [nowhere dense](../../../topological-analysis.md#nowhere-dense-set).

There are countably many [integer](../../../number-theory.md#integer) tuples, and $\mathbb R^n$ is complete. The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) therefore makes the complement of their union [dense](../../../topology.md#dense-set) and nonempty. Choosing any point there gives

$$
\boxed{\sum_{j=1}^nk_jx_j\ne k_{n+1}\quad\text{for every nonzero integer tuple }k.}
$$

Equivalently, $1,x_1,\ldots,x_n$ are [linearly independent](../../../vector-space.md#linear-independence) over $\mathbb Q$: multiplying a rational relation by a common denominator produces just such an [integer](../../../number-theory.md#integer) relation. This is an instance of [Baire avoidance of countably many affine hyperplanes](../../../topological-analysis.md#baire-avoidance-of-countably-many-affine-hyperplanes).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and normalized measure $dt/(2\pi)$. The [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum) at zero is the real [linear functional](../../../linear-algebra.md#linear-functional)

$$
L_Nf=S_N(f,0)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)D_N(t)\,dt,
$$

where the [Dirichlet kernel](../../../fourier-series.md#dirichlet-kernel) is

$$
D_N(t)=\sum_{j=-N}^Ne^{ijt}=\frac{\sin((N+\tfrac12)t)}{\sin(t/2)}.
$$

The quotient follows by summing the finite [geometric progression](../../../real-analysis.md#geometric-progression), with its removable value $D_N(0)=2N+1$. It is a real [continuous](../../../calculus.md#continuous-function) [periodic function](../../../function.md#periodic-function). If

$$
\Lambda_N=\frac1{2\pi}\int_{-\pi}^{\pi}|D_N(t)|\,dt,
$$

then $|L_Nf|\leq\Lambda_N\|f\|_\infty$. This bound is its exact [operator norm](../../../continuous-dual-space.md#operator-norm) even on the real [continuous](../../../calculus.md#continuous-function) functions. Indeed, for $\delta>0$ set

$$
f_{N,\delta}(t)=\frac{D_N(t)}{\sqrt{D_N(t)^2+\delta^2}}.
$$

It is real, [continuous](../../../calculus.md#continuous-function) and periodic with [norm](../../../functional-analysis.md#norm) at most one, and

$$
L_Nf_{N,\delta}=\frac1{2\pi}\int_{-\pi}^{\pi}
\frac{D_N(t)^2}{\sqrt{D_N(t)^2+\delta^2}}\,dt\longrightarrow\Lambda_N
$$

by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem). At zeros of the kernel the integrand is zero, and elsewhere its limit is $|D_N|$.

For $0<t\leq\pi$, $\sin(t/2)\leq t/2$. Using evenness and putting $v=(N+1/2)t$ gives

$$
\Lambda_N\geq\frac2\pi\int_0^{(N+1/2)\pi}\frac{|\sin v|}{v}\,dv
\geq\frac4{\pi^2}\sum_{j=1}^N\frac1j.
$$

For the last inequality, split into the first $N$ complete intervals $[(j-1)\pi,j\pi]$: their sine integrals are two and $1/v\geq1/(j\pi)$. The [harmonic sum](../../../real-analysis.md#harmonic-sum) tends to infinity. This proves the [Dirichlet kernel harmonic lower bound](../../../fourier-series.md#dirichlet-kernel-harmonic-lower-bound).

Choose $N$ with $\Lambda_N>K$, then choose $\delta$ sufficiently small that $L_Nf_{N,\delta}>K$. Thus

$$
\boxed{\|f_{N,\delta}\|_\infty\leq1,\qquad |S_N(f_{N,\delta},0)|>K.}
$$

This constructs [continuous](../../../calculus.md#continuous-function) near-maximizers, rather than using the discontinuous sign of the kernel as the desired function.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

The real space $C(\mathbb T)$ is a [Banach space](../../../banach-space.md) in the [uniform norm](../../../functional-analysis.md#supremum-norm): a uniformly [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) has a uniform pointwise limit by [completeness](../../../topological-analysis.md#completeness) of $\mathbb R$, and that [uniform limit](../../../real-analysis.md#uniform-limit) is [continuous](../../../calculus.md#continuous-function). Each functional $L_N$ from the preceding part is bounded, but their norms are unbounded.

For integers $m\geq1$, define

$$
E_m=\{f\in C(\mathbb T):|L_Nf|\leq m\text{ for every }N\}.
$$

Each $E_m$ is [closed](../../../topology.md#closed-set), being an intersection of inverse images of [closed](../../../topology.md#closed-set) intervals under [continuous](../../../calculus.md#continuous-function) functionals. It has empty interior. Otherwise some ball $B(f_0,r)$ would be contained in it. For every $h$ of [norm](../../../functional-analysis.md#norm) at most one, both $f_0$ and $f_0+(r/2)h$ would belong to that ball, so

$$
\frac r2|L_Nh|\leq |L_N(f_0+(r/2)h)|+|L_Nf_0|\leq2m.
$$

Taking the [supremum](../../../real-analysis.md#supremum) over $h$ would give $\|L_N\|\leq4m/r$ for all $N$, contradicting the preceding part.

Thus the $E_m$ are [nowhere dense](../../../topological-analysis.md#nowhere-dense-set). The [Baire category theorem](../../../topological-analysis.md#baire-category-theorem) says their union cannot cover $C(\mathbb T)$. A function outside that union satisfies

$$
\boxed{\sup_N|S_N(f,0)|=\infty,}
$$

so its [Fourier series](../../../fourier-series.md) diverges at zero. In fact these functions form a [dense](../../../topology.md#dense-set) $G_\delta$ subset of $C(\mathbb T)$. This proves the relevant [Uniform boundedness principle](../../../banach-space.md#uniform-boundedness-principle) argument directly and establishes [generic unbounded Fourier sums at a fixed point](../../../fourier-series.md#generic-unbounded-fourier-sums-at-a-fixed-point).

## 2

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The hypotheses make $p$ a [sublinear functional](../../../functional-analysis.md#sublinear-function) and $q$ a [superlinear functional](../../../functional-analysis.md#superlinear-functional). In particular $p(0)=q(0)=0$. Apply the domination property to $y+y'\in Y$ and the vector $x+x'$:

$$
S(y)+S(y')\leq p(x+x'+y+y')-q(x+x').
$$

[Subadditivity](../../../real-analysis.md#subadditive-sequence) of $p$, with the inserted vectors $z$ and $-z$, gives

$$
p(x+x'+y+y')\leq p(x+y+z)+p(x'+y'-z).
$$

Superadditivity of $q$ gives $q(x+x')\geq q(x)+q(x')$. Combining these inequalities and moving terms yields exactly

$$
\boxed{S(y')-p(x'+y'-z)+q(x')
\leq-S(y)+p(x+y+z)-q(x).}
$$

Every vector appearing in the comparison is permitted by the assumed domination, so no membership of $x,x',z$ in $Y$ is needed.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

We prove the extension by [Zorn's lemma](../../../set-theory.md#zorn-s-lemma), retaining the full domination condition. Consider all pairs $(Y,S)$ extending $(Y_0,T_0)$, with $Y$ a subspace and $S$ linear, satisfying $S(y)\leq p(x+y)-q(x)$ for every $x\in X,y\in Y$. Order these pairs by extension. A chain has an upper bound: take the union of its subspaces and maps. The union is a subspace, and its map is well defined and linear because any finitely many vectors lie together in one member of the chain. Its domination is inherited there. Thus a maximal extension exists.

Suppose its domain $Y$ is proper, and choose $z\notin Y$. A linear extension to $Y+\mathbb Rz$ has the form $S_a(y+tz)=S(y)+ta$. Define the [admissible values for a sandwich extension](../../../functional-analysis.md#admissible-values-for-a-sandwich-extension) by

$$
A=\sup_{x',y'}\{S(y')-p(x'+y'-z)+q(x')\},
$$



$$
B=\inf_{x,y}\{-S(y)+p(x+y+z)-q(x)\},
$$

with $x,x'\in X$ and $y,y'\in Y$. Part (i) shows every quantity in the [supremum](../../../real-analysis.md#supremum) is at most every quantity in the [infimum](../../../real-analysis.md#infimum), hence $A\leq B$. Both bounds are real and finite: choosing zero vectors provides $A\geq-p(-z)$ and $B\leq p(z)$, and the pairwise comparison then bounds them from the other sides. Choose $a\in[A,B]$.

For $t>0$, [positive homogeneity](../../../real-analysis.md#positively-homogeneous-function-degree-one) and the upper bound on $a$, used with $x/t,y/t$, give

$$
S(y)+ta\leq t\big[p(x/t+y/t+z)-q(x/t)\big]
=p(x+y+tz)-q(x).
$$

For $t=-s<0$, the lower bound on $a$ applied to $x/s,y/s$ gives

$$
a\geq S(y/s)-p(x/s+y/s-z)+q(x/s),
$$

which rearranges to $S(y)-sa\leq p(x+y-sz)-q(x)$. For $t=0$ this is the existing domination. Thus $S_a$ is a legitimate larger extension, contradicting maximality. The maximal domain is therefore all of $X$; call its map $T$.

Setting the first vector in the domination to zero yields $T(v)\leq p(v)$. Setting it to $v$ and the domain vector to $-v$ yields $-T(v)\leq-q(v)$. Consequently

$$
\boxed{T|_{Y_0}=T_0,\qquad T(y)\leq p(x+y)-q(x),\qquad q(v)\leq T(v)\leq p(v).}
$$

The one-dimensional extension has checked both signs of its coefficient; [positive homogeneity](../../../real-analysis.md#positively-homogeneous-function-degree-one) alone does not permit treating negative coefficients as positive ones.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Take $Y_0=\{0\}$ and $T_0(0)=0$. The hypothesis $p(x)\geq q(x)$ is exactly the required initial domination $0\leq p(x+0)-q(x)$. Applying the extension proved in part (ii) gives

$$
\boxed{q(x)\leq U(x)\leq p(x)\quad\text{for every }x\in X,}
$$

with $U$ linear. There is no reason that $U$ must be nonzero; for instance $p=q=0$ forces $U=0$.

This is the [sandwich form of the Hahn-Banach theorem](../../../functional-analysis.md#sandwich-form-of-the-hahn-banach-theorem). Conversely, any [linear map](../../../vector-space.md#linear-map) between these two functionals satisfies the stronger mixed domination, since $U(y)=U(x+y)-U(x)\leq p(x+y)-q(x)$. Thus the mixed inequality used during extension is the appropriate invariant, not an extra final restriction.

## 3

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use a nonzero complex unital [Banach algebra](../../../banach-algebra.md) $B$ with submultiplicative [norm](../../../functional-analysis.md#norm), and write its [unit](../../../algebra.md#unit-in-a-ring) as $e$. The complex [scalar field](../../../quantum-field-theory.md#scalar-field) is the usual convention in this spectral statement; for a real algebra one uses its complexification. We derive the needed analytic facts from norm-convergent series and scalar complex analysis.

If $\|a\|<1$, [completeness](../../../topological-analysis.md#completeness) makes the [Neumann series](../../../banach-algebra.md#neumann-series) $\sum_{j=0}^\infty a^j$ converge. Multiplying its finite partial sums by $e-a$ gives $e-a^{m+1}$, which tends to $e$. Hence its sum is the inverse of $e-a$. If $b$ is invertible, then $b+h=b(e+b^{-1}h)$ is invertible whenever $\|b^{-1}h\|<1$. This proves that the invertible elements form an [open set](../../../topology.md#open-set) and that inversion is locally norm-continuous.

Define the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) and the [resolvent of an element](../../../banach-algebra.md#resolvent-of-an-element) by

$$
\sigma(x)=\{\lambda\in\mathbb C:\lambda e-x\text{ is not invertible}\},
\qquad R(\lambda)=(\lambda e-x)^{-1}\quad(\lambda\notin\sigma(x)).
$$

For $|\lambda|>\|x\|$, the [Neumann series](../../../banach-algebra.md#neumann-series) gives

$$
\boxed{R(\lambda)=\sum_{j=0}^\infty\frac{x^j}{\lambda^{j+1}},\qquad x^0=e.}
$$

Thus $\sigma(x)$ is bounded by $\|x\|$ and is [closed](../../../topology.md#closed-set), because invertibility is open. Also $R(\lambda)\to0$ in [norm](../../../functional-analysis.md#norm) at infinity; for example its [norm](../../../functional-analysis.md#norm) is at most $\|e\|/(|\lambda|-\|x\|)$, since $\|e\|\geq1$ in a nonzero submultiplicative unital algebra. The standard normalization $\|e\|=1$ is not needed.

For points where the [Banach algebra resolvent](../../../banach-algebra.md#resolvent-of-an-element) exists $\lambda,\mu$, multiply out the inverses to get the [resolvent identity](../../../banach-algebra.md#resolvent-identity)

$$
\boxed{R(\lambda)-R(\mu)=(\mu-\lambda)R(\lambda)R(\mu).}
$$

For $\lambda_0$ outside the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element), put $R_0=R(\lambda_0)$. Locally,

$$
R(\lambda_0+h)=R_0(e+hR_0)^{-1}
=\sum_{j=0}^\infty(-h)^jR_0^{j+1},\qquad |h|\|R_0\|<1.
$$

This series and its differentiated series converge uniformly on every smaller disk. It therefore proves $R$ is a [Banach-space-valued holomorphic function](../../../complex-analysis.md#banach-space-valued-holomorphic-function), establishing complex differentiability in the Banach-space [norm](../../../functional-analysis.md#norm) and gives $R'=-R^2$, without assuming a Banach-algebra-valued analytic theorem. In particular every [continuous](../../../calculus.md#continuous-function) complex [linear functional](../../../linear-algebra.md#linear-functional) $\phi$ makes $\phi(R(\lambda))$ a scalar [holomorphic function](../../../complex-analysis.md#holomorphic-function).

The [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is nonempty. Otherwise $R$ would be defined and analytic everywhere. Its local [norm](../../../functional-analysis.md#norm) continuity and decay at infinity make it globally bounded. For every [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) $\phi$, the scalar [entire function](../../../complex-analysis.md#entire-function) $\phi(R(\lambda))$ is bounded and tends to zero at infinity, so it is identically zero: the scalar [Cauchy estimate](../../../analysis.md#cauchy-estimate) for its [derivative](../../../calculus.md#derivative) on circles of radius $r$ is $M/r$, which tends to zero, and the limiting value then fixes its constant as zero. Such functionals separate points by the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem). Explicitly a bounded real functional can be extended from the real span of any nonzero element using its [norm](../../../functional-analysis.md#norm), and complexifying it by $\phi(v)=\ell(v)-i\ell(iv)$ gives a bounded complex [linear functional](../../../linear-algebra.md#linear-functional) nonzero on that element. Therefore $R$ itself would be zero, contradicting $(\lambda e-x)R=e$. We have proved **the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is a nonempty compact subset of the [complex plane](../../../complex-analysis.md#complex-plane)**.

We next establish the [spectral radius formula](../../../analysis.md#spectral-radius-formula). The power norms are submultiplicative. If some $x^m=0$, their root norms are eventually zero. Otherwise, for any fixed $m$, write $n=qm+r$ with $0\leq r<m$ to obtain

$$
\|x^n\|\leq\|x^m\|^q\max_{0\leq r<m}\|x^r\|.
$$

Taking roots gives $\limsup_n\|x^n\|^{1/n}\leq\|x^m\|^{1/m}$. Taking the [infimum](../../../real-analysis.md#infimum) in $m$, and using that every root [norm](../../../functional-analysis.md#norm) is at least that [infimum](../../../real-analysis.md#infimum), proves existence of

$$
\rho_0=\lim_{n\to\infty}\|x^n\|^{1/n}
=\inf_{m\geq1}\|x^m\|^{1/m}.
$$

For $|\lambda|>\rho_0$, the [root test](../../../real-analysis.md#root-test) makes $\sum x^j/\lambda^{j+1}$ converge, even when $|\lambda|\leq\|x\|$. The same telescoping [multiplication](../../../arithmetic.md#multiplication) proves it is a two-sided inverse. Hence

$$
r_\sigma:=\max_{\lambda\in\sigma(x)}|\lambda|\leq\rho_0.
$$

For the reverse bound fix $R>r_\sigma$. If $R_1>\max(R,\|x\|)$, integrate the uniformly convergent exterior series term by term on $|\lambda|=R_1$, obtaining

$$
x^n=\frac1{2\pi i}\int_{|\lambda|=R_1}\lambda^nR(\lambda)\,d\lambda.
$$

The same integral equals the one on $|\lambda|=R$: applying an arbitrary [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) reduces [contour deformation](../../../complex-analysis.md#contour-deformation) through the [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element)-free annulus to the scalar [Cauchy theorem](../../../complex-analysis.md#cauchy-s-integral-theorem), and separation of points restores equality in $B$. This proves the [resolvent Cauchy coefficient formula](../../../banach-algebra.md#resolvent-cauchy-coefficient-formula) rather than assuming vector-valued analytic calculus. Using the [norm](../../../functional-analysis.md#norm) bound for the allowed vector integral gives

$$
\|x^n\|\leq R^{n+1}\max_{|\lambda|=R}\|R(\lambda)\|.
$$

Taking $n$th roots yields $\rho_0\leq R$, and letting $R\downarrow r_\sigma$ finishes the proof:

$$
\boxed{\rho(x)=\lim_{n\to\infty}\|x^n\|^{1/n}
=\max_{\lambda\in\sigma(x)}|\lambda|
=\sup\{|\lambda|:\lambda e-x\text{ is not invertible}\}.}
$$

For the first example take the [commutative algebra](../../../commutative-algebra.md) of [dual numbers](../../../commutative-algebra.md#dual-number) $B=\mathbb C[\varepsilon]/(\varepsilon^2)$ with [norm](../../../functional-analysis.md#norm) $\|a+b\varepsilon\|=|a|+|b|$. [Completeness](../../../topological-analysis.md#completeness) follows from finite dimension, and the product estimate makes the [norm](../../../functional-analysis.md#norm) submultiplicative. For $x=\varepsilon$, $x\ne0$ but $x^2=0$, so $\rho(x)=0$. Directly, $\lambda e-\varepsilon$ has inverse $\lambda^{-1}e+\lambda^{-2}\varepsilon$ for $\lambda\ne0$, and its [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is $\{0\}$. For the second example take $B=\mathbb C$ with its absolute-value [norm](../../../functional-analysis.md#norm) and $x=1$. Its [Banach algebra spectrum](../../../banach-algebra.md#spectrum-of-an-element) is $\{1\}$, giving **$\rho(x)=\|x\|=1$**.

## 4

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

We construct the finite evaluation representation explicitly by [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial). This supplies all the [polynomial](../../../polynomial.md) facts needed for the bound.

Define the [Chebyshev polynomial](../../../numerical-analysis.md#chebyshev-polynomial) by $T_0=1,T_1=x$ and

$$
T_{m+1}(x)=2xT_m(x)-T_{m-1}(x).
$$

Induction shows that $T_m$ has degree $m$; the [cosine](../../../geometry-and-topology.md#cosine) addition identity also proves $T_m(\cos\theta)=\cos(m\theta)$. Therefore $\|T_n\|_{[-1,1]}=1$, and $T_n(-x)=(-1)^nT_n(x)$ follows from the recurrence. The case $n=0$ is immediate, since both $P$ and $T_0$ are constant.

For $n\geq1$, choose the descending extremal nodes

$$
x_j=\cos(j\pi/n),\qquad 0\leq j\leq n,
$$

so $T_n(x_j)=(-1)^j$. Define the fundamental interpolation polynomials

$$
\ell_j(t)=\prod_{k\ne j}\frac{t-x_k}{x_j-x_k}.
$$

They satisfy $\ell_j(x_k)=\delta_{jk}$. Consequently

$$
\boxed{P(t)=\sum_{j=0}^nP(x_j)\ell_j(t)}
$$

for every [polynomial](../../../polynomial.md) of degree at most $n$: the difference has degree at most $n$ and vanishes at the $n+1$ distinct nodes, so it is zero. The root count used here follows by successively factoring $(t-x_j)$ from a [polynomial](../../../polynomial.md) having such a root; a nonzero degree-$n$ [polynomial](../../../polynomial.md) cannot have more than $n$ distinct roots. Thus the interpolation identity has been proved.

If $u>1$, every numerator factor in $\ell_j(u)$ is positive, while exactly $j$ denominator factors are negative. Hence $\operatorname{sgn}\ell_j(u)=(-1)^j$. Applying interpolation to $T_n$ itself gives

$$
\sum_{j=0}^n|\ell_j(u)|=\sum_{j=0}^n(-1)^j\ell_j(u)=T_n(u)>0.
$$

Putting $M=\sup_{[-1,1]}|P|$ in the interpolation formula yields

$$
|P(u)|\leq\sum_{j=0}^n|P(x_j)||\ell_j(u)|\leq M T_n(u).
$$

For $u<-1$, apply the proved positive-side inequality to $Q(t)=P(-t)$ at $-u>1$, and use the parity identity. The result is

$$
\boxed{|P(u)|\leq\|P\|_{[-1,1]}|T_n(u)|,\qquad u\notin[-1,1].}
$$

This is sharp, with equality for $P=T_n$ or its scalar multiples.

In functional terms, the evaluation map $E_u:P\mapsto P(u)$ on the normed [polynomial](../../../polynomial.md) space has $\|E_u\|=|T_n(u)|$: the inequality gives the upper bound and $T_n$ attains it. For $u>1$, its normalized version has the exact representation

$$
\frac{E_u(P)}{T_n(u)}=\sum_{j=0}^n\lambda_jP(x_j),
\qquad\lambda_j=\frac{\ell_j(u)}{T_n(u)},\quad
\sum_{j=0}^n|\lambda_j|=1.
$$

Thus [Chebyshev interpolation represents external evaluation](../../../numerical-analysis.md#chebyshev-interpolation-represents-external-evaluation) using $n+1$ nodes. The necessary finite representation and its [norm](../../../functional-analysis.md#norm) are derived directly, so no convex-hull theorem is being invoked without proof.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
