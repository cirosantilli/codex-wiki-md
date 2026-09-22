# Paper 6

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper6.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper6.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

First scale the stated unit-ball approximation. For every nonzero residual $r\in F$, apply the hypothesis to $r/\|r\|$ and multiply the resulting vector by $\|r\|$. This gives $v\in E$ with

$$
\|v\|\le R\|r\|,\qquad \|Tv-r\|\le k\|r\|.
$$

For zero residual use $v=0$. Start with $r_0=y$, choose $v_j$ by this rule for $r_j$, and set $r_{j+1}=r_j-Tv_j$. Inductively,

$$
\|r_j\|\le k^j\|y\|,\qquad \|v_j\|\le Rk^j\|y\|.
$$

The [Banach space](../../../banach-space.md) $E$ therefore contains the sum $x=\sum_{j\ge0}v_j$, with

$$
\boxed{\|x\|\le\frac R{1-k}\|y\|.}
$$

The partial sums satisfy $T\sum_{j=0}^{n-1}v_j=y-r_n$. Boundedness of $T$ gives convergence of the left side to $Tx$, while $r_n\to0$ gives $Tx=y$. Thus **$T$ is [surjective](../../../algebra.md#surjective-function) with the stated lifting bound**. This [geometric correction for approximate surjectivity](../../../functional-analysis.md#geometric-correction-for-approximate-surjectivity) used [completeness](../../../topological-analysis.md#completeness) of $E$, not any unproved [completeness](../../../topological-analysis.md#completeness) of $F$.

Put $C=R/(1-k)$. Given a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) $(y_n)$ in $F$, choose a subsequence $(y_{n_j})$ such that $\|y_{n_{j+1}}-y_{n_j}\|\le2^{-j}$ for $j\ge1$. Lift each difference to $u_j\in E$ with $Tu_j=y_{n_{j+1}}-y_{n_j}$ and $\|u_j\|\le C2^{-j}$. Lift $y_{n_1}$ to $u_0$. The sum $u=u_0+\sum_{j\ge1}u_j$ exists in $E$, and its image is the limit of the subsequence. A [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) with a convergent subsequence converges to the same limit: use the [triangle inequality](../../../topological-analysis.md#triangle-inequality) between an arbitrary late term, a later subsequence term, and the limit. This proves **$F$ is complete**, the [completeness forced by uniformly bounded lifting](../../../functional-analysis.md#completeness-forced-by-uniformly-bounded-lifting) principle.

The [open mapping theorem](../../../functional-analysis.md#open-mapping-theorem-functional-analysis) states that a bounded [surjective](../../../algebra.md#surjective-function) linear operator between [Banach spaces](../../../banach-space.md) maps open sets to open sets. In particular a bounded linear bijection between [Banach spaces](../../../banach-space.md) has a bounded inverse. To deduce the [closed graph theorem](../../../functional-analysis.md#closed-graph-theorem), let $S:E_1\to F_1$ be an everywhere-defined [linear map](../../../vector-space.md#linear-map) between [Banach spaces](../../../banach-space.md) with closed graph. Its graph is a closed subspace of the Banach product $E_1\times F_1$, with [norm](../../../functional-analysis.md#norm) $\|(x,y)\|=\|x\|+\|y\|$, so it is itself Banach. The projection

$$
\pi_1:\operatorname{graph}S\to E_1,\qquad(x,Sx)\mapsto x
$$

is a bounded linear bijection. The [open mapping theorem](../../../functional-analysis.md#open-mapping-theorem-functional-analysis) makes its inverse bounded. Composing that inverse with the bounded second projection proves that $S$ is bounded. This is the required closed graph conclusion, rather than a continuity assumption on $S$.

Finally consider the identity map $I:(C(X),\|\cdot\|)\to(C(X),\|\cdot\|_\infty)$. If $f_n\to f$ in the new [norm](../../../functional-analysis.md#norm) and $f_n\to g$ uniformly, each assumed continuous [point evaluation functional](../../../topological-vector-space.md#point-evaluation-functional) gives $f_n(x)\to f(x)$, while [uniform convergence](../../../real-analysis.md#uniform-convergence) gives $f_n(x)\to g(x)$. Hence $f=g$. Since both spaces are metric, this sequential argument proves the graph is closed. Both [norms](../../../functional-analysis.md#norm) are complete, so the [closed graph theorem](../../../functional-analysis.md#closed-graph-theorem) makes $I$ bounded. Its inverse is bounded by the [open mapping theorem](../../../functional-analysis.md#open-mapping-theorem-functional-analysis). Consequently there are constants $c,C'>0$ such that

$$
\boxed{c\|f\|_\infty\le\|f\|\le C'\|f\|_\infty\qquad(f\in C(X)).}
$$

This proves [Banach norm rigidity from continuous point evaluations](../../../functional-analysis.md#banach-norm-rigidity-from-continuous-point-evaluations). Pointwise continuity alone would not give a common bound on all evaluations; [completeness](../../../topological-analysis.md#completeness) supplies that through the closed graph argument.

## 2

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A point $x$ of a [convex set](../../../mathematical-optimization.md#convex-set) $K$ is an [extreme point](../../../mathematical-optimization.md#extreme-point) if $x=(1-t)a+tb$ with $a,b\in K$ and $0<t<1$ forces $a=b=x$. It is enough to test midpoints: a nontrivial interior point of a segment is the midpoint of a smaller nontrivial segment.

Here is a proof of the [Krein-Milman theorem](../../../functional-analysis.md#krein-milman-theorem). The empty-set case is immediate, so take $K\ne\varnothing$. A [face of a convex set](../../../mathematical-optimization.md#face-of-a-convex-set) is a convex subset $F\subseteq K$ such that an interior convex combination lying in $F$ has both endpoints in $F$. Consider nonempty compact faces. They include $K$. Every inclusion chain has nonempty intersection, because its closed subsets of the compact set $K$ have the [finite intersection property](../../../topology.md#finite-intersection-property). The intersection remains a compact face. The [Zorn lemma](../../../set-theory.md#zorn-s-lemma), ordered by reverse inclusion, therefore supplies a minimal nonempty compact face $F$.

If $F$ contains two distinct points, the Hausdorff locally convex hypotheses and the allowed separation theorem supply a continuous real [linear functional](../../../linear-algebra.md#linear-functional) $\ell$ taking different values there. Its maximizer set in $F$ is nonempty and compact. It is convex, and if a convex combination attains the maximum, both endpoint values attain it too; hence it is a face of $F$. A face of a face is a face of $K$, by applying the defining endpoint property twice. This maximizer face is proper because $\ell$ is nonconstant, contradicting minimality. Thus $F$ is a singleton, whose point is extreme in $K$. The same [minimal compact face argument](../../../functional-analysis.md#minimal-compact-face-argument) inside any nonempty compact face shows that each such face contains an [extreme point](../../../mathematical-optimization.md#extreme-point) of $K$.

Let $H=\overline{\operatorname{conv}}(\operatorname{ext}K)$. Since $K$ is compact, hence closed in the [Hausdorff space](../../../topology.md#hausdorff-space), and convex, $H\subseteq K$. It is nonempty, closed and convex. If $p\in K\setminus H$, the allowed strict separation theorem supplies a continuous [linear functional](../../../linear-algebra.md#linear-functional) with

$$
\ell(p)>\sup_{h\in H}\ell(h).
$$

The maximizer face of $\ell$ on $K$ contains an [extreme point](../../../mathematical-optimization.md#extreme-point) $e$ by the preceding argument. Then $e\in H$ but $\ell(e)=\max_K\ell\ge\ell(p)>\sup_H\ell$, a contradiction. Therefore

$$
\boxed{K=\overline{\operatorname{conv}}(\operatorname{ext}K).}
$$

All closures refer to the given locally convex topology, and [compactness](../../../topology.md#compact-space) is what justified both maxima and chain intersections.

For the real [l-infinity sequence space](../../../banach-space.md#l-infinity-sequence-space), if $|x_j|<1$ for any coordinate, choose $0<\epsilon\le1-|x_j|$. The two distinct sequences $x\pm\epsilon e_j$ belong to the closed unit ball and have midpoint $x$, so $x$ is not extreme. Conversely, if every $x_j$ is one or minus one, writing $x=(1-t)a+tb$ for unit-ball sequences forces $a_j=b_j=x_j$ at every coordinate, because an endpoint of $[-1,1]$ cannot be a nontrivial convex average of its points. Thus

$$
\boxed{\operatorname{ext}B_{\ell^\infty}=\{-1,1\}^{\mathbb N}.}
$$

For the [space of sequences converging to zero](../../../functional-analysis.md#space-of-sequences-converging-to-zero), every unit-ball sequence has some coordinate with $|x_j|<1$, since its coordinates tend to zero. The same opposite single-coordinate perturbations still belong to $c_0$, giving

$$
\boxed{\operatorname{ext}B_{c_0}=\varnothing.}
$$

These are [extreme points of real sequence-space unit balls](../../../mathematical-optimization.md#extreme-points-of-real-sequence-space-unit-balls). There is no conflict with Krein-Milman: the norm-closed unit ball of $c_0$ is not [compact](../../../topology.md#compact-space) in the [norm topology](../../../functional-analysis.md#norm-topology), as the coordinate vectors have mutual distance one.

## 3

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Work with a nonzero complex unital [Banach algebra](../../../banach-algebra.md), so $1\ne0$. The [spectrum of an element](../../../banach-algebra.md#spectrum-of-an-element) is

$$
\sigma_A(x)=\{\lambda\in\mathbb C:\lambda1-x\text{ is not invertible in }A\}.
$$

For $|\lambda|>\|x\|$, the [Neumann series](../../../banach-algebra.md#neumann-series)

$$
(\lambda1-x)^{-1}=\sum_{n=0}^{\infty}\frac{x^n}{\lambda^{n+1}}
$$

converges in [norm](../../../functional-analysis.md#norm) and is a two-sided inverse, by multiplying its partial sums and letting the remainder tend to zero. Thus the [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) lies in $|\lambda|\le\|x\|$. The assumed openness of the invertible group makes its complement closed, so the [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) is compact.

To prove nonemptiness, suppose every $\lambda$ has an inverse $R(\lambda)=(\lambda1-x)^{-1}$. Locally,

$$
R(\lambda+h)=R(\lambda)(1+hR(\lambda))^{-1}
=\sum_{j\ge0}(-h)^jR(\lambda)^{j+1},
$$

so the resolvent is holomorphic. At infinity its [Neumann series](../../../banach-algebra.md#neumann-series) gives $\|R(\lambda)\|=O(|\lambda|^{-1})$. For any [bounded linear functional](../../../topological-vector-space.md#continuous-linear-functional) $\ell\in A^*$, the scalar [entire function](../../../complex-analysis.md#entire-function) $\ell(R(\lambda))$ is bounded: it is bounded on compact disks by continuity, and tends to zero outside them. The [Liouville theorem](../../../complex-analysis.md#liouville-theorem) makes it constant, and its limit makes that constant zero. The [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) separates points of the normed space $A$, so $R(\lambda)=0$, contradicting $(\lambda1-x)R(\lambda)=1$. Hence **the [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) is nonempty and compact**.

On the algebra of [entire functions](../../../complex-analysis.md#entire-function), set

$$
\boxed{\|f\|_D=\sup_{|z|\le1}|f(z)|.}
$$

It is finite, homogeneous and satisfies the [triangle inequality](../../../topological-analysis.md#triangle-inequality) and [submultiplicativity](../../../banach-algebra.md#submultiplicativity). If it vanishes, the [identity theorem](../../../complex-analysis.md#identity-theorem) makes $f$ identically zero, so it is an [algebra norm](../../../banach-algebra.md#algebra-norm). However, no [algebra norm](../../../banach-algebra.md#algebra-norm) on the entire-function algebra can be complete. The coordinate function $Z(z)=z$ satisfies $\sigma(Z)=\mathbb C$ algebraically: $Z-\lambda$ vanishes at $z=\lambda$ and has no entire multiplicative inverse. A complete [algebra norm](../../../banach-algebra.md#algebra-norm) would make this a [Banach algebra](../../../banach-algebra.md), contradicting the proved boundedness of its [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis). This is the [entire function algebra admits no complete algebra norm](../../../banach-algebra.md#entire-function-algebra-admits-no-complete-algebra-norm) obstruction; it applies to every proposed complete [algebra norm](../../../banach-algebra.md#algebra-norm), not only the displayed one.

For all [continuous functions](../../../calculus.md#continuous-function) on $\mathbb C$, choose continuous cutoffs

$$
h_n(z)=\begin{cases}
1,&|z-3n|\le1/2,\\
2(1-|z-3n|),&1/2<|z-3n|<1,\\
0,&|z-3n|\ge1.
\end{cases}
$$

Their supports are disjoint and escape every compact set. Thus $f(z)=\sum_{n\ge1}nh_n(z)$ is a locally finite sum and is continuous. Let $g_n(z)=\max(0,1-4|z-3n|)$. This nonzero [continuous function](../../../calculus.md#continuous-function) is supported where $h_n=1$ and all the other cutoffs vanish. Hence $fg_n=ng_n$. Any [algebra norm](../../../banach-algebra.md#algebra-norm) would imply

$$
n\|g_n\|=\|fg_n\|\le\|f\|\|g_n\|,
$$

so $n\le\|f\|$ for every positive integer, impossible. Therefore **the algebra of all [continuous functions](../../../calculus.md#continuous-function) on $\mathbb C$ admits no [algebra norm](../../../banach-algebra.md#algebra-norm)**, even an incomplete one. This proves the [continuous functions on the complex plane admit no algebra norm](../../../banach-algebra.md#continuous-functions-on-the-complex-plane-admit-no-algebra-norm) obstruction directly.

## 4

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Set $a_n=\|x^n\|$ and $D=\inf_{n\ge1}a_n^{1/n}$. If some $x^m=0$, all later powers vanish, their root [norms](../../../functional-analysis.md#norm) tend to zero, and $D=0$. Otherwise fix $m\ge1$ and write $n=qm+s$, $0\le s<m$. [Submultiplicativity](../../../banach-algebra.md#submultiplicativity) gives

$$
a_n\le a_m^q C_m,\qquad C_m=\max_{0\le s<m}\|x^s\|.
$$

Since $q/n\to1/m$, it follows that $\limsup_na_n^{1/n}\le a_m^{1/m}$. Taking the infimum over $m$ and using $a_n^{1/n}\ge D$ proves

$$
\lim_{n\to\infty}\|x^n\|^{1/n}=D.
$$

This establishes existence of the limit and its infimum characterization before identifying it with the [spectral radius](../../../analysis.md#spectral-radius) $r(x)=\max_{\lambda\in\sigma(x)}|\lambda|$.

For $|\lambda|>D$, the [root test](../../../real-analysis.md#root-test) makes $\sum_{n\ge0}x^n/\lambda^{n+1}$ converge absolutely. Multiplication of partial sums shows that its limit is $(\lambda1-x)^{-1}$. Thus $r(x)\le D$. For the reverse inequality, take any $\rho>r(x)$ and the circle $|\lambda|=\rho$. The [resolvent of an element](../../../banach-algebra.md#resolvent-of-an-element) is holomorphic off the [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis), and

$$
x^n=\frac1{2\pi i}\int_{|\lambda|=\rho}\lambda^n(\lambda1-x)^{-1}\,d\lambda.
$$

To justify this identity, first use a radius larger than $\|x\|$ and integrate the uniformly convergent [Neumann series](../../../banach-algebra.md#neumann-series) term by term. Then deform to radius $\rho$: the intervening annulus has no spectral points. The [Cauchy theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) for these Banach-valued integrals follows by applying [bounded linear functionals](../../../topological-vector-space.md#continuous-linear-functional) and using their point separation. Consequently, with $M_\rho=\max_{|\lambda|=\rho}\|(\lambda1-x)^{-1}\|$,

$$
\|x^n\|\le\rho^{n+1}M_\rho.
$$

Taking root limits gives $D\le\rho$; let $\rho\downarrow r(x)$. Hence the full [spectral radius formula](../../../analysis.md#spectral-radius-formula) is

$$
\boxed{r(x)=\lim_{n\to\infty}\|x^n\|^{1/n}
=\inf_{n\ge1}\|x^n\|^{1/n}.}
$$

For the product comparison, if $\lambda\ne0$ and $R=(\lambda1-xy)^{-1}$, direct multiplication on both sides verifies

$$
(\lambda1-yx)^{-1}=\lambda^{-1}(1+yRx).
$$

Indeed $(\lambda1-yx)y=y(\lambda1-xy)$, and the remaining terms cancel against the inverse equation. Interchanging $x,y$ proves the converse. Thus the [nonzero spectra of products in opposite orders](../../../banach-algebra.md#nonzero-spectra-of-products-in-opposite-orders) agree, so

$$
\boxed{r(xy)=r(yx).}
$$

The possible difference at zero has no effect on the maximum modulus, including when that maximum is zero.

Zero really can differ. In $A=\mathcal B(\ell^2(\mathbb N_0))$, let $S$ be the [unilateral shift operator](../../../linear-operator-theory.md#unilateral-shift-operator), $Se_n=e_{n+1}$, and take $x=S^*$, $y=S$. Then $xy=1$, whereas $yx=1-P_0$, with $P_0$ the projection onto $e_0$. The latter is zero on $e_0$ and identity on its orthogonal complement, and these blocks also explicitly invert it away from zero and one. Hence

$$
\boxed{\sigma(xy)=\{1\},\qquad\sigma(yx)=\{0,1\}.}
$$

Finally, for $t>r(x)$ the root [norms](../../../functional-analysis.md#norm) of $(x/t)^n$ tend to $r(x)/t<1$, so their [norms](../../../functional-analysis.md#norm) eventually decay geometrically and the powers converge to zero. Conversely, if the powers converge to zero, choose $N$ with $\|(x/t)^N\|<1$. Homogeneity and the infimum formula imply

$$
\frac{r(x)}t\le\|(x/t)^N\|^{1/N}<1,
$$

so $t>r(x)$. The admissible positive $t$ are exactly $(r(x),\infty)$, proving the [power-decay characterization of the spectral radius](../../../analysis.md#power-decay-characterization-of-the-spectral-radius)

$$
\boxed{r(x)=\inf\{t>0:(t^{-1}x)^n\to0\}.}
$$

This includes quasinilpotent elements with radius zero; no positive endpoint must be attained.

## 5

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Write $K=\sigma_A(x)$ and $R_x(\zeta)=(\zeta1-x)^{-1}$. Suppose first that a unital complex-algebra homomorphism sends $Z$ to $x$. If $\lambda\notin U$, the [holomorphic function](../../../complex-analysis.md#holomorphic-function) $1/(Z-\lambda)$ belongs to $\mathcal O(U)$ and is the multiplicative inverse of $Z-\lambda$. Its image is an inverse for $x-\lambda1$. Thus **existence forces $K\subset U$**, even before continuity is used.

For the converse, assume $K\subset U$. Choose a bounded finite union of polygonal regions $V$ with $K\subset V$, $\overline V\subset U$, and boundary avoiding $K$. Orient its boundary cycle $\Gamma$ positively around $V$, including negative orientations on holes. Its winding number is one near $K$ and zero outside $U$. Define

$$
\boxed{\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(\zeta)R_x(\zeta)\,d\zeta.}
$$

The integral exists in $A$ because the integrand is continuous on finitely many compact contour pieces. The [Cauchy theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) shows it is unchanged by replacing $\Gamma$ with another such spectral cycle: the difference has zero winding around the possible singularities in $K$. Banach-valued Cauchy statements follow by applying [bounded linear functionals](../../../topological-vector-space.md#continuous-linear-functional). We use the scalar [Cauchy integral formula](../../../analysis.md#cauchy-integral-formula) in its cycle form: a cycle with index one at a point and surrounding only a holomorphy region integrates $f(\zeta)/(\zeta-z)$ to $2\pi i f(z)$.

Linearity is immediate and, for a fixed cycle,

$$
\|\Theta_x(f)\|\le\frac{\operatorname{length}\Gamma}{2\pi}
\max_\Gamma\|R_x(\zeta)\|\,\sup_\Gamma|f|.
$$

This is a bound by one compact-uniform seminorm, proving continuity for [local uniform convergence](../../../real-analysis.md#locally-uniform-convergence). To obtain $\Theta_x(1)=1$, deform the resolvent integral, which is holomorphic on $\mathbb C\setminus K$, to a large circle and integrate its [Neumann series](../../../banach-algebra.md#neumann-series). Similarly $\zeta R_x(\zeta)=1+xR_x(\zeta)$ gives $\Theta_x(Z)=x$.

For multiplicativity choose an outer spectral cycle for $f$ and an inner one for $g$, nested in $U$ so the inner cycle lies inside the outer region. The [resolvent identity](../../../banach-algebra.md#resolvent-identity) is

$$
R_x(\zeta)R_x(\eta)=\frac{R_x(\eta)-R_x(\zeta)}{\zeta-\eta}.
$$

Substitute it into the double integral for $\Theta_x(f)\Theta_x(g)$. In the term containing $R_x(\eta)$, first integrate $f(\zeta)/(\zeta-\eta)$ around the outer cycle, obtaining $f(\eta)$. In the term containing $R_x(\zeta)$, first integrate $g(\eta)/(\zeta-\eta)$ around the inner cycle, obtaining zero because $\zeta$ lies outside it. Interchange is valid for the continuous integrands on disjoint compact cycles. Hence

$$
\Theta_x(f)\Theta_x(g)=\Theta_x(fg).
$$

This proves the required continuous unital homomorphism, the [holomorphic functional calculus](../../../banach-algebra.md#holomorphic-functional-calculus).

For uniqueness use the following version of the allowed [Runge theorem](../../../complex-analysis.md#runge-s-theorem): on any open $U\subseteq\mathbb C$, [rational functions](../../../isolated-singularity.md#rational-function) with all finite poles outside $U$ approximate each [holomorphic function](../../../complex-analysis.md#holomorphic-function) locally uniformly; poles at infinity are allowed, giving [polynomials](../../../polynomial.md). A unital homomorphism sending $Z$ to $x$ is forced on [polynomials](../../../polynomial.md) and on every inverse $(Z-\lambda)^{-1}$, $\lambda\notin U$, and hence on these [rational functions](../../../isolated-singularity.md#rational-function). Continuity then forces its value on their limits. Thus **$\Theta_x$ is unique**. This argument works for disconnected $U$ as well and does not assume [polynomials](../../../polynomial.md) alone are dense. It proves [continuity and uniqueness of holomorphic functional calculus](../../../banach-algebra.md#continuity-and-uniqueness-of-holomorphic-functional-calculus).

We will use the character description of [spectra](../../../linear-operator-theory.md#spectrum-functional-analysis), with a short justification. A [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) $\varphi$ is a nonzero complex multiplicative [linear functional](../../../linear-algebra.md#linear-functional); it satisfies $\varphi(1)=1$. Applying it to an inverse shows $\varphi(a)\in\sigma_A(a)$, so $|\varphi(a)|\le\|a\|$ and the character is automatically continuous. Conversely, for noninvertible $a-\lambda1$, its [principal ideal](../../../commutative-algebra.md#principal-ideal) is proper because $A$ is commutative. Put it in a [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $M$. The closure of $M$ is proper: an ideal containing an element sufficiently close to one contains an invertible element and thus the identity. Maximality makes $M$ closed. The quotient is a complex Banach division algebra. By the nonempty-spectrum result of Question 3, each quotient element differs from some scalar by a noninvertible element, which in a division algebra must be zero. Thus the quotient is $\mathbb C$ and its quotient map is a character taking $a$ to $\lambda$. This proves

$$
\sigma_A(a)=\{\varphi(a):\varphi\text{ a character of }A\}.
$$

It is the [spectrum equals character values in a commutative Banach algebra](../../../banach-algebra.md#spectrum-equals-character-values-in-a-commutative-banach-algebra) statement and does not assume semisimplicity.

For any character, continuity permits passing it inside the contour integral. Since $\varphi(R_x(\zeta))=(\zeta-\varphi(x))^{-1}$ and $\varphi(x)\in K$, the scalar Cauchy formula gives

$$
\boxed{\varphi(\Theta_x(f))=\frac1{2\pi i}\int_\Gamma
\frac{f(\zeta)}{\zeta-\varphi(x)}\,d\zeta=f(\varphi(x)).}
$$

Apply the character description first to $\Theta_x(f)$ and then to $x$ to obtain the [holomorphic spectral mapping theorem](../../../mathematics.md#holomorphic-spectral-mapping-theorem)

$$
\boxed{\sigma_A(\Theta_x(f))=f(\sigma_A(x)).}
$$

On $\Pi_+$, use the analytic logarithm with argument in $(-\pi/2,\pi/2)$ and set $s(z)=\exp(\tfrac12\operatorname{Log} z)$. It satisfies $s(z)^2=z$ and takes its values in $\Pi_+$. The [principal square root in a commutative Banach algebra](../../../banach-algebra.md#principal-square-root-in-a-commutative-banach-algebra) is

$$
\boxed{y=\Theta_x(s),\qquad y^2=x,\qquad\sigma_A(y)\subset\Pi_+.}
$$

For uniqueness let $v$ be another root with [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) in $\Pi_+$. For each character, $\varphi(y)$ and $\varphi(v)$ are scalar roots of $\varphi(x)$ with positive real part, so both equal $s(\varphi(x))$. Hence every character takes the nonzero value $2s(\varphi(x))$ at $y+v$. The character description implies $y+v$ is invertible. Commutativity gives $(y-v)(y+v)=y^2-v^2=0$, and multiplying by the inverse yields $y=v$. Equal character values alone would not imply equality in a possibly nonsemisimple algebra; the invertible sum is the essential extra step.

## 6

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

First the [C-star identity](../../../banach-algebra.md#c-star-identity) and [submultiplicativity](../../../banach-algebra.md#submultiplicativity) give $\|a\|^2=\|a^*a\|\le\|a^*\|\|a\|$, hence $\|a\|\le\|a^*\|$ when $a\ne0$. Applying this to $a^*$ gives equality, so the [involution](../../../group-theory.md#involution) is isometric and continuous. Also $\|1\|=\|1\|^2$ and $1\ne0$, yielding $\|1\|=1$.

For a [Normal element of a C-star algebra](../../../banach-algebra.md#normal-element-of-a-c-star-algebra) $x$, put $b=x^*x$, which is a [self-adjoint C-star element](../../../banach-algebra.md#hermitian-element-of-a-c-star-algebra). Normality gives $(x^*)^2x^2=b^2$, and the [C-star identity](../../../banach-algebra.md#c-star-identity) applied to $x^2$ and to $b$ gives

$$
\|x^2\|^2=\|(x^*)^2x^2\|=\|b^2\|=\|b\|^2=\|x\|^4.
$$

Thus $\|x^2\|=\|x\|^2$. Every power of $x$ is normal because $x$ commutes with $x^*$, so iteration yields

$$
\|x^{2^j}\|=\|x\|^{2^j}\qquad(j\ge0).
$$

The [spectral radius formula](../../../analysis.md#spectral-radius-formula) has a limit along all positive integers, and along this subsequence its root [norms](../../../functional-analysis.md#norm) are exactly $\|x\|$. Therefore

$$
\boxed{r(x)=\|x\|.}
$$

This proves [spectral radius norm equality for normal elements](../../../banach-algebra.md#spectral-radius-norm-equality-for-normal-elements) directly from the defining [norm](../../../functional-analysis.md#norm) identity, rather than assuming a spectral representation in advance.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Let $h=h^*$. The exponential $u_t=e^{ith}$ is defined by its norm-convergent power series. Continuity and conjugate linearity of the [involution](../../../group-theory.md#involution) give $u_t^*=e^{-ith}$, and multiplication of the commuting exponential series gives $u_t^*u_t=u_tu_t^*=1$. Thus $u_t$ is a [Unitary element of a C-star algebra](../../../banach-algebra.md#unitary-element-of-a-c-star-algebra) and, by the [C-star identity](../../../banach-algebra.md#c-star-identity), $\|u_t\|=1$.

A [character of an algebra](../../../banach-algebra.md#character-of-an-algebra) is automatically continuous with $|\varphi(a)|\le\|a\|$, as proved in Question 5. Passing it through the exponential series gives

$$
|e^{it\varphi(h)}|=|\varphi(u_t)|\le1\qquad(t\in\mathbb R).
$$

The left side is $e^{-t\Im\varphi(h)}$. Considering both signs of $t$ forces $\Im\varphi(h)=0$. So characters take real values on [self-adjoint C-star elements](../../../banach-algebra.md#hermitian-element-of-a-c-star-algebra).

Now write $x=h+ik$ with

$$
h=\frac{x+x^*}{2},\qquad k=\frac{x-x^*}{2i},
$$

both [self-adjoint C-star elements](../../../banach-algebra.md#hermitian-element-of-a-c-star-algebra). Then

$$
\boxed{\varphi(x^*)=\varphi(h)-i\varphi(k)=\overline{\varphi(h)+i\varphi(k)}=\overline{\varphi(x)}.}
$$

This proves that [characters of a C-star algebra respect the involution](../../../banach-algebra.md#characters-of-a-c-star-algebra-respect-the-involution). The argument itself does not require commutativity, although a noncommutative algebra need not have any characters.

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For the unheaded representation request, retain the question's standing unital hypothesis. Let $K$ be the [character space of an algebra](../../../banach-algebra.md#character-space-of-an-algebra) of $A$, with its weak-star or [Gelfand topology](../../../banach-algebra.md#gelfand-topology). The standard commutative Banach-algebra results allowed here give a nonempty compact Hausdorff [character space](../../../banach-algebra.md#character-space-of-an-algebra) and $\sigma_A(a)=\{\varphi(a):\varphi\in K\}$. In particular, character [compactness](../../../topology.md#compact-space) follows from the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem): the equations $\varphi(1)=1$ and $\varphi(ab)=\varphi(a)\varphi(b)$ define a weak-star closed subset of the dual unit ball.

The [Gelfand transform](../../../banach-algebra.md#gelfand-representation) is the unital homomorphism

$$
\Gamma:A\to C(K),\qquad \Gamma(a)(\varphi)=\varphi(a).
$$

Every element of the commutative [C-star algebra](../../../banach-algebra.md#c-star-algebra) is normal. Part i and the character [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) formula therefore give

$$
\|\Gamma(a)\|_\infty=\max_{\varphi\in K}|\varphi(a)|=r(a)=\|a\|.
$$

Thus $\Gamma$ is an isometry, hence injective, and its range is closed because $A$ is complete. Part ii gives $\Gamma(a^*)=\overline{\Gamma(a)}$. The range contains constants and separates points of $K$, since two distinct characters differ on some element of $A$. The complex [Stone-Weierstrass theorem](../../../functional-analysis.md#stone-weierstrass-theorem) states that a unital, conjugation-closed subalgebra of $C(K)$ separating points of a compact [Hausdorff space](../../../topology.md#hausdorff-space) is uniformly dense. Its application here, together with closedness of the range, yields

$$
\boxed{\Gamma:A\overset{\cong}{\longrightarrow}C(K)\text{ is an isometric }*\text{-isomorphism}.}
$$

This proves the [Commutative Gelfand--Naimark theorem](../../../banach-algebra.md#commutative-gelfand-naimark-theorem) from the preceding parts and the stated approximation theorem.

The word “every” in the printed deduction must be read under the initial unital hypothesis. If nonunital commutative [C-star algebras](../../../banach-algebra.md#c-star-algebra) are included, the compact-space statement is false: the nonzero algebra $c_0$ has no multiplicative identity, whereas $C(K)$ for nonempty compact $K$ does. The general nonunital version is $C_0(K)$ on a locally compact [Hausdorff space](../../../topology.md#hausdorff-space), with vanishing at infinity. This qualification preserves the proved unital result.

For the final [real spectrum criterion for a normal C-star element](../../../banach-algebra.md#real-spectrum-criterion-for-a-normal-c-star-element), the ambient algebra may be noncommutative. Let $B$ be the norm-closed unital subalgebra generated by $x$ and $x^*$. Normality makes these two generators commute. The [involution](../../../group-theory.md#involution) preserves their [polynomial](../../../polynomial.md) algebra and is continuous, so $B$ is a commutative [C-star subalgebra](../../../banach-algebra.md#c-star-subalgebra).

We first show that $x$ has the same [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) in $B$ as in $A$, without assuming spectral permanence. Put $\Omega=\mathbb C\setminus\sigma_A(x)$. A compact subset of the real axis has connected complement: upper and lower half-plane paths join around either end of a bounded interval containing it, and each omitted real point can be joined locally to the upper half-plane. Define

$$
V=\{\lambda\in\Omega:(\lambda1-x)^{-1}\in B\}.
$$

This set is nonempty because the [Neumann series](../../../banach-algebra.md#neumann-series) puts the inverse in $B$ for $|\lambda|>\|x\|$. It is relatively open: from an inverse in $B$, the local inverse formula

$$
R(\lambda+h)=R(\lambda)\sum_{n\ge0}[-hR(\lambda)]^n
$$

stays in $B$ for small $h$. It is relatively closed by continuity of the ambient resolvent and norm-closedness of $B$. Connectedness gives $V=\Omega$. Conversely an inverse in $B$ is an inverse in $A$, so

$$
\sigma_B(x)=\sigma_A(x)\subset\mathbb R.
$$

This is the connected-resolvent case of [spectrum in a closed unital subalgebra](../../../banach-algebra.md#spectrum-in-a-closed-unital-subalgebra).

Apply the just-proved commutative C-star representation to $B$. For every character $\psi$ of $B$, $\psi(x)$ lies in this real [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis). Part ii makes $\psi(x^*)=\overline{\psi(x)}=\psi(x)$. The [Gelfand transform](../../../banach-algebra.md#gelfand-representation) of $B$ is injective by its isometry, so

$$
\boxed{x=x^*.}
$$

For a nonunital ambient [C-star algebra](../../../banach-algebra.md#c-star-algebra), perform the same argument in its standard [C-star unitization](../../../banach-algebra.md#unitization-of-a-c-star-algebra), using the usual [unitization](../../../banach-algebra.md#unitization-of-an-algebra) [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis).

Normality cannot be dropped. In $M_2(\mathbb C)$, take

$$
N=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
$$

Since $N^2=0$, its [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) is $\{0\}$: for $\lambda\ne0$, $(\lambda I-N)^{-1}=\lambda^{-1}I+\lambda^{-2}N$, while $N$ is not invertible. Yet $N\ne N^*$ and

$$
NN^*=\begin{pmatrix}1&0\\0&0\end{pmatrix}\ne
\begin{pmatrix}0&0\\0&1\end{pmatrix}=N^*N.
$$

Thus **a real [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) alone does not force self-adjointness; normality is essential**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
