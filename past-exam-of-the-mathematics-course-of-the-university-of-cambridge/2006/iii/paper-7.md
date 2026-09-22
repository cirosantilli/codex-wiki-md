# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper7.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Identify the [circle](../../../topology.md#circle) with $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and use normalized [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) and [convolution](../../../fourier-analysis.md#convolution):

$$
\widehat f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-int}\,dt,\qquad (f*g)(t)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t-s)g(s)\,ds.
$$

For $0\leq r<1$, summing two [geometric series](../../../real-analysis.md#geometric-series) gives the [Poisson kernel on the circle](../../../partial-differential-equation.md#poisson-kernel-on-the-circle):

$$
1+\sum_{n\geq1}r^n(e^{int}+e^{-int})=\frac1{1-re^{it}}+\frac1{1-re^{-it}}-1=\frac{1-r^2}{1-2r\cos t+r^2}=P_r(t).
$$

This [Fourier series](../../../fourier-series.md) converges absolutely and uniformly for each fixed $r<1$. Consequently we can integrate it term by term in the [convolution](../../../fourier-analysis.md#convolution); the substitution $u=t-s$ gives

$$
\boxed{(f*P_r)(t)=\sum_{n\in\mathbb Z}\widehat f(n)r^{|n|}e^{int}.}
$$

The resulting series is itself absolutely and uniformly convergent, since $|\widehat f(n)|\leq\|f\|_\infty$ and $\sum_n r^{|n|}<\infty$.

The [Poisson kernel on the circle](../../../partial-differential-equation.md#poisson-kernel-on-the-circle) is nonnegative and has normalized integral one, as its constant [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) is one. Its mass concentrates near zero. Indeed, for $r\geq1/2$ and $\delta\leq|s|\leq\pi$,

$$
0\leq P_r(s)=\frac{1-r^2}{(1-r)^2+2r(1-\cos s)}\leq\frac{1-r^2}{1-\cos\delta}.
$$

Hence its normalized integral outside $(-\delta,\delta)$ tends to zero as $r\uparrow1$. Given $\eta>0$, [uniform continuity](../../../topological-analysis.md#uniform-continuity) of $f$ gives a $\delta>0$ such that $|f(t-s)-f(t)|<\eta$ whenever the circular distance of $s$ from zero is less than $\delta$. Splitting the [convolution](../../../fourier-analysis.md#convolution) error into this arc and its complement yields

$$
\sup_t|(f*P_r)(t)-f(t)|\leq\eta+2\|f\|_\infty\frac1{2\pi}\int_{\delta\leq|s|\leq\pi}P_r(s)\,ds.
$$

The second term tends to zero, and $\eta$ is arbitrary. Thus **the Abel sums converge uniformly to $f$**, or $\boxed{\|f*P_r-f\|_\infty\to0}$. This is [uniform Poisson summability of continuous circle functions](../../../partial-differential-equation.md#uniform-poisson-summability-of-continuous-circle-functions): positivity, unit mass and concentration supply the required [approximate identity](../../../fourier-analysis.md#approximate-identity) argument.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Use the given integer $u$ satisfying $u^2\equiv-1\pmod p$. The [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) under consideration has basis $(1,u),(0,p)$, because every vector in it is uniquely $(a,ua+bp)$ with $a,b\in\mathbb Z$. Its fundamental parallelogram therefore has area

$$
\left|\det\begin{pmatrix}1&0\\u&p\end{pmatrix}\right|=p.
$$

We use the following two-dimensional form of the [Minkowski convex body theorem](../../../algebraic-number-theory.md#minkowski-s-theorem): a convex, centrally symmetric measurable subset of $\mathbb R^2$ of area strictly greater than four times the covolume of a full-rank [Euclidean lattice](../../../fourier-analysis.md#euclidean-lattice) contains a nonzero vector of that lattice. Apply it to the closed disk of squared radius $3p/2$. Its area is $3\pi p/2>4p$, so it contains a nonzero lattice vector $(a,b)$ satisfying

$$
0<a^2+b^2\leq\frac{3p}{2}<2p.
$$

On the other hand the defining [modular congruence](../../../number-theory.md#modular-congruence) and $u^2\equiv-1\pmod p$ imply

$$
a^2+b^2\equiv a^2+(ua)^2=(1+u^2)a^2\equiv0\pmod p.
$$

There is exactly one positive multiple of $p$ strictly below $2p$, so $\boxed{p=a^2+b^2}$. Neither coordinate can be zero, since a prime is not the square of an integer. This [congruence lattice proof of the prime sum of two squares](../../../number-theory.md#congruence-lattice-proof-of-the-prime-sum-of-two-squares) proves the required case of the [sum of two squares theorem](../../../number-theory.md#sum-of-two-squares-theorem) without assuming any conclusion at the critical area $4p$.

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $S_Nf(t)=\sum_{|n|\leq N}\widehat f(n)e^{int}$ for the symmetric [Fourier partial sum](../../../fourier-series.md#fourier-partial-sum), with normalized [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) on $\mathbb T=\mathbb R/(2\pi\mathbb Z)$. We will prove the stronger conclusion

$$
\boxed{\limsup_{N\to\infty}|S_Nf(t)|=\infty\quad\text{for every }t\in E.}
$$

If $E$ is empty, take $f=0$. Otherwise the proof of the [Kahane-Katznelson divergence theorem](../../../fourier-series.md#kahane-katznelson-divergence-theorem) has three steps: a bounded [trigonometric polynomial](../../../fourier-series.md#trigonometric-polynomial) whose partial sum is large on short arcs, a finite-arc batching of an arbitrary null set, and a uniformly convergent sequence of separated frequency blocks. In particular, no assumption that $E$ is closed or compact is needed.

First consider a nonempty finite family of arcs with centers $\theta_\nu$, half-lengths $0<d_\nu\leq1$, and $D=\sum_\nu d_\nu$. On the closed unit disk define

$$
\Phi(z)=\sum_\nu\frac{d_\nu}{D}\frac{1+d_\nu}{1+d_\nu-ze^{-i\theta_\nu}}.
$$

Each summand has positive real part there, and $\Phi(0)=1$. Thus the principal [complex logarithm](../../../analysis.md#complex-logarithm) $A=\log\Phi$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on a neighborhood of the closed disk, $A(0)=0$, and $|\operatorname{Im}A|<\pi/2$. To bound its real part on an arc, put $h=t-\theta_\nu$ with $|h|\leq d_\nu$ and $q=1+d_\nu-\cos h$. Then

$$
d_\nu\leq q\leq\tfrac32d_\nu,\qquad |\sin h|\leq d_\nu,\qquad \operatorname{Re}\frac{1+d_\nu}{1+d_\nu-e^{ih}}=\frac{(1+d_\nu)q}{q^2+\sin^2h}\geq\frac4{13d_\nu}>\frac1{4d_\nu}.
$$

After multiplication by the weight $d_\nu/D$, this contribution is at least $1/(4D)$; all the other contributions have positive real part. Throughout the arc union we therefore have

$$
\operatorname{Re}\Phi(e^{it})\geq\frac1{4D},\qquad \operatorname{Re}A(e^{it})=\log|\Phi(e^{it})|\geq\log\frac1{4D}.
$$

This is the [positive-real logarithmic amplifier for short arcs](../../../fourier-series.md#positive-real-logarithmic-amplifier-for-short-arcs). Since $A$ is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) beyond the closed unit disk, its [Taylor series](../../../calculus.md#taylor-series) converges uniformly there. Choose a polynomial $Q(z)=\sum_{\nu=1}^{d}a_\nu z^\nu$ with $\sup_{|z|\leq1}|Q(z)-A(z)|<1$. There is no constant term because $A(0)=0$. Set $C=\pi/2+1$ and

$$
B(t)=\operatorname{Im}Q(e^{it})=\frac{Q(e^{it})-\overline{Q(e^{it})}}{2i},\qquad P(t)=\frac{e^{iMt}}C B(t),
$$

where the integer $M>d$ may be chosen arbitrarily large. We have $\|P\|_\infty\leq1$, and its frequencies lie in $[M-d,M+d]$. At the cut $N=M$, the positive-frequency half of $Q$ is excluded and the negative-frequency half is included. Hence

$$
S_MP(t)=-\frac{e^{iMt}}{2iC}\overline{Q(e^{it})},\qquad |S_MP(t)|\geq\frac{\log(1/(4D))-1}{2C}
$$

on the arc union. In particular, for any $K>0$, a total half-length $D\leq\tfrac14e^{-1-2CK}$ gives $|S_MP|\geq K$ there. This proves the needed [compact-set Fourier amplification lemma](../../../fourier-series.md#compact-set-fourier-amplification-lemma), with the additional freedom to place its entire frequency block above any prescribed frequency.

Next we construct the [null-set limsup cover by finite arc families](../../../measure-theory.md#null-set-limsup-cover-by-finite-arc-families). Set

$$
a_j=2^{-j},\qquad K_j=2^j(j+2),\qquad D_j=\tfrac14e^{-1-2CK_j}\quad(j\geq1).
$$

Since $E$ has [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) zero, for every row $\ell\geq1$ choose a countable arc cover $\{I_{\ell,m}:m\geq1\}$ of $E$ with positive half-lengths $d_{\ell,m}$ and $\sum_m d_{\ell,m}<2^{-\ell}D_1$. We can take closed arcs by slightly enlarging an open cover; their half-lengths are less than one. The whole two-index array has total half-length less than $D_1$. Absolute convergence of this sum lets us choose strictly increasing integers $N_j$ such that the sum outside the finite square $1\leq\ell,m\leq N_j$ is less than $D_{j+1}$. Put $N_0=0$ and let $\mathcal F_j$ contain those arcs for which

$$
N_{j-1}<\max(\ell,m)\leq N_j.
$$

Each family is finite. Its total half-length is less than $D_j$: for $j=1$ use the total sum, and for $j>1$ use the tail outside the preceding square. Moreover, every $t\in E$ belongs to arcs with unbounded row index, so belongs to the unions of infinitely many of the families $\mathcal F_j$. This batching is essential: a dense null set need not have a finite cover of small total length, whereas the infinitely-often finite covers above suffice.

Apply the amplification construction to $\mathcal F_j$ with height $K_j$, obtaining $P_j$ with $\|P_j\|_\infty\leq1$ and $|S_{M_j}P_j(t)|\geq K_j$ on that family's union. Choose the modulation integers successively so that the frequency intervals $[M_j-d_j,M_j+d_j]$ are positive and each lies strictly above the preceding one. Empty families may be represented by $P_j=0$ and an unused frequency interval. Define the [frequency-separated Fourier block series](../../../fourier-series.md#frequency-separated-fourier-block-series)

$$
f(t)=\sum_{j=1}^{\infty}a_jP_j(t).
$$

The bound $\sum_j a_j\|P_j\|_\infty\leq1$ gives absolute [uniform convergence](../../../real-analysis.md#uniform-convergence), so $f$ is continuous. Uniform convergence also justifies computing every [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) term by term. At frequency $M_j$, all earlier blocks have been included in full and all later blocks are absent:

$$
S_{M_j}f(t)=\sum_{i<j}a_iP_i(t)+a_jS_{M_j}P_j(t).
$$

For $t$ in the union of $\mathcal F_j$, the reverse [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
|S_{M_j}f(t)|\geq a_jK_j-\sum_{i<j}a_i\geq j+1.
$$

Every $t\in E$ lies in infinitely many such unions, and $M_j\to\infty$. Therefore the boxed unboundedness holds at every point of $E$, completing the proof for arbitrary null sets.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use the angular-frequency [Fourier transform](../../../analysis.md#fourier-transform) convention

$$
\widehat f(\lambda)=\int_{\mathbb R}f(x)e^{-i\lambda x}\,dx.
$$

A precise sufficient interpretation of the regularity assumption is $f\ne0$, $f\in H^1(\mathbb R)$ in the [first-order Sobolev space](../../../sobolev-space.md#first-order-sobolev-space) and $xf\in L^2(\mathbb R)$; in particular, nonzero [Schwartz functions](../../../fourier-analysis.md#schwartz-function) are admissible. We use the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem), in the normalization $\|\widehat f\|_2^2=2\pi\|f\|_2^2$, together with its derivative identity $\widehat{f'}(\lambda)=i\lambda\widehat f(\lambda)$. Both identities hold in $L^2$ for $f\in H^1$, by extending their identities for [Schwartz functions](../../../fourier-analysis.md#schwartz-function). Thus the frequency factor is

$$
\frac{\int\lambda^2|\widehat f(\lambda)|^2\,d\lambda}{\int|\widehat f(\lambda)|^2\,d\lambda}=\frac{\|f'\|_2^2}{\|f\|_2^2}.
$$

For a [Schwartz function](../../../fourier-analysis.md#schwartz-function), [integration by parts](../../../calculus.md#integration-by-parts) gives $\|f\|_2^2=-2\operatorname{Re}\int x f'(x)\overline{f(x)}\,dx$. This remains true under the stated assumptions: insert a smooth cutoff $\chi_R(x)=\chi(x/R)$ into the derivative of $x|f|^2$, where $\chi$ is one near zero and compactly supported. Integration gives

$$
\int(\chi_R+x\chi_R')|f|^2\,dx=-2\operatorname{Re}\int\chi_R x f'\overline f\,dx.
$$

The cutoff-derivative term tends to zero, since $x\chi_R'$ is bounded independently of $R$ and supported in a tail. The other terms converge by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) and the integrability of $|f'||xf|$, furnished by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Hence

$$
\|f\|_2^2=-2\operatorname{Re}\langle f',xf\rangle\leq2|\langle f',xf\rangle|\leq2\|f'\|_2\|xf\|_2.
$$

After squaring and using the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem), we obtain the [uncentred Fourier uncertainty principle](../../../analysis.md#uncentred-fourier-uncertainty-principle):

$$
\boxed{\frac{\int x^2|f(x)|^2\,dx}{\int|f(x)|^2\,dx}\frac{\int\lambda^2|\widehat f(\lambda)|^2\,d\lambda}{\int|\widehat f(\lambda)|^2\,d\lambda}\geq\frac14.}
$$

If equality holds, both displayed inequalities must be equalities. The equality condition in the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $f'=cxf$ almost everywhere for a constant $c\in\mathbb C$; the real-part inequality and the identity for $\|f\|_2^2$ then force $c=-a$ with $a>0$ real. The [weak derivative](../../../distribution-theory.md#weak-derivative) equation has the solution $f(x)=C e^{-ax^2/2}$: locally multiply by $e^{ax^2/2}$ to obtain a function whose weak derivative is zero, hence a constant. Conversely, for this [Gaussian function](../../../calculus.md#gaussian-function) the normalized second moments are $1/(2a)$ in position and $a/2$ in angular frequency, whose product is $1/4$. Therefore

$$
\boxed{\text{Equality holds exactly for }f(x)=C e^{-ax^2/2},\quad a>0,\ C\in\mathbb C\setminus\{0\}.}
$$

These are raw second moments, rather than variances about their respective means. Consequently translations and nonzero frequency modulations of the [Gaussian function](../../../calculus.md#gaussian-function) are not equality cases here; the [equality case of the Heisenberg uncertainty relation](../../../quantum-theory.md#equality-case-of-the-heisenberg-uncertainty-relation) for centred variances has those additional freedoms.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Use $\widehat f(\lambda)=\int f(t)e^{-i\lambda t}\,dt$ and interpret the regularity assumption to include $f\in L^2(\mathbb R)$ with the continuous representative furnished by [Fourier inversion](../../../fourier-analysis.md#fourier-inversion-theorem). Write $F=\widehat f$. The bandwidth assumption implies $F\in L^1$ as well as $L^2$, by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) on its finite support, so

$$
f(t)=\frac1{2\pi}\int_{-\pi}^{\pi}F(\lambda)e^{it\lambda}\,d\lambda
$$

is continuous and defined at every $t$. The integer samples are precisely the [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) of $F$ with the sign convention appropriate to the basis $e^{-in\lambda}$:

$$
f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}F(\lambda)e^{in\lambda}\,d\lambda.
$$

The completeness and [Parseval identity](../../../fourier-analysis.md#parseval-identity) for the exponential [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) on $[-\pi,\pi]$ give $F=\sum_{n\in\mathbb Z}f(n)e^{-in\lambda}$ in $L^2$ and

$$
\sum_{n\in\mathbb Z}|f(n)|^2=\frac1{2\pi}\|F\|_2^2=\|f\|_2^2.
$$

The last equality is the [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem). Apply the inverse integral to the finite symmetric [Fourier partial sums](../../../fourier-series.md#fourier-partial-sum). Since

$$
\frac1{2\pi}\int_{-\pi}^{\pi}e^{i(t-n)\lambda}\,d\lambda=\frac{\sin\pi(t-n)}{\pi(t-n)},
$$

we obtain the [Nyquist–Shannon sampling theorem](../../../fourier-analysis.md#nyquist-shannon-sampling-theorem) in this normalization:

$$
\boxed{f(t)=\sum_{n\in\mathbb Z}f(n)\frac{\sin\pi(t-n)}{\pi(t-n)}\quad(t\in\mathbb R),}
$$

where the quotient is one at $t=n$. This is a [sampling expansion by periodic Fourier projection](../../../fourier-analysis.md#sampling-expansion-by-periodic-fourier-projection), not merely an almost-everywhere inversion. Indeed, the inverse integral of an error $G\in L^2[-\pi,\pi]$ is bounded, uniformly in $t$, by $\|G\|_2/\sqrt{2\pi}$. Hence the symmetric finite sampling sums converge uniformly on all of $\mathbb R$. Moreover, the [Parseval identity](../../../fourier-analysis.md#parseval-identity) applied to $e^{it\lambda}$ gives

$$
\sum_{n\in\mathbb Z}\left|\frac{\sin\pi(t-n)}{\pi(t-n)}\right|^2=1.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) therefore makes the sampling series absolutely convergent at every $t$, with its absolute tail bounded uniformly by $(\sum_{|n|>N}|f(n)|^2)^{1/2}$. Thus the integer samples recover the function everywhere.

For the nonuniqueness beyond this bandwidth, fix $0<\epsilon_0<\min(\epsilon,\pi)$ and a nonzero smooth function $\Phi$ compactly supported in $(-\epsilon_0,\epsilon_0)$. Let $h$ be its inverse [Fourier transform](../../../analysis.md#fourier-transform) and put

$$
g(t)=\sin(\pi t)h(t),\qquad \widehat g(\lambda)=\frac{\Phi(\lambda-\pi)-\Phi(\lambda+\pi)}{2i}.
$$

The function $h$, and hence $g$, is a [Schwartz function](../../../fourier-analysis.md#schwartz-function). The two shifted spectral supports are disjoint, so $\widehat g\ne0$, but its support is contained strictly inside $(-\pi-\epsilon,\pi+\epsilon)$. Every integer sample of $g$ is zero. Therefore **$g$ and the zero function have identical samples but are distinct**, providing a [strictly supercritical sampling alias counterexample](../../../fourier-analysis.md#strictly-supercritical-sampling-alias-counterexample) for every positive bandwidth enlargement.

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For the [Riemann-Lebesgue lemma](../../../fourier-analysis.md#riemann-lebesgue-lemma), a half-period shift of the oscillation gives a direct proof. For a nonzero integer $r$, set $h=\pi/r$. Periodicity and a change of variable show that the [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) of $t\mapsto f(t+h)$ at $r$ is $e^{irh}\widehat f(r)=-\widehat f(r)$. Thus

$$
2\widehat f(r)=\frac1{2\pi}\int_{-\pi}^{\pi}(f(t)-f(t+h))e^{-irt}\,dt,\qquad |\widehat f(r)|\leq\frac12\sup_t|f(t)-f(t+\pi/r)|.
$$

The right side tends to zero as $|r|\to\infty$ by [uniform continuity](../../../topological-analysis.md#uniform-continuity) on the [circle](../../../topology.md#circle). Consequently $\boxed{\widehat f(r)\to0\text{ as }|r|\to\infty}$.

There is nevertheless no prescribed rate shared by all continuous functions. Choose increasing positive integers $n_j$ with $k(n_j)\geq j2^j$, which is possible since $k(r)\to\infty$. Define

$$
g(t)=\sum_{j=1}^{\infty}2^{-j}e^{in_jt}.
$$

The series converges absolutely and uniformly, so $g$ is continuous. Termwise integration is justified by [uniform convergence](../../../real-analysis.md#uniform-convergence), and the orthogonality of distinct exponential modes gives $\widehat g(n_j)=2^{-j}$. Hence

$$
k(n_j)|\widehat g(n_j)|\geq j,\qquad \boxed{\limsup_{r\to\infty}k(r)|\widehat g(r)|=\infty.}
$$

This [arbitrarily slow Fourier coefficient decay](../../../fourier-analysis.md#arbitrarily-slow-fourier-coefficient-decay) is compatible with the [Riemann-Lebesgue lemma](../../../fourier-analysis.md#riemann-lebesgue-lemma): for this particular function all [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) still tend to zero, but along the selected subsequence they beat the proposed decay scale by an unbounded factor.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Put $L=2\pi$ and represent the [circle](../../../topology.md#circle) by $[0,L)$. The full [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [Haar wavelets](../../../fourier-analysis.md#haar-wavelet) includes the constant $H_*=L^{-1/2}$ and, for every dyadic interval $I$ of length $\ell=L2^{-j}$, the normalized detail

$$
H_I=\ell^{-1/2}(\mathbf1_{I_{\mathrm{left}}}-\mathbf1_{I_{\mathrm{right}}}),\qquad c_I=\int_0^Lf(t)\overline{H_I(t)}\,dt.
$$

Take half-open intervals and the corresponding values at their boundaries, so every point belongs to exactly one interval at each level. The constant basis function is necessary: if it were omitted, even $f\equiv1$ could not satisfy the asserted convergence. We use the full conventional [Haar wavelet](../../../fourier-analysis.md#haar-wavelet) system in the threshold sum.

Let $A_Jf$ be the function equal to the mean of $f$ on each level-$J$ dyadic interval. Comparing the means on a parent and its two children proves the [Haar refinement identity](../../../fourier-analysis.md#haar-refinement-identity) directly: the difference between the child mean and the parent mean is the appropriate value of $c_IH_I$. Inductively this gives the [Haar projection](../../../fourier-analysis.md#haar-projection)

$$
A_Jf=c_*H_*+\sum_{j=0}^{J-1}\sum_{I\text{ at level }j}c_IH_I,\qquad c_*H_*=\frac1L\int_0^Lf(t)\,dt.
$$

Writing $\omega_f(s)=\sup_{\operatorname{dist}(x,y)\leq s}|f(x)-f(y)|$ for the [modulus of continuity](../../../topological-analysis.md#modulus-of-continuity), the cell-average formula yields

$$
\|A_Jf-f\|_\infty\leq\omega_f(L2^{-J})\longrightarrow0.
$$

For a detail on a cell $I$, its integral is zero. Subtracting $f(x_I)$ for any $x_I\in I$ therefore gives the coefficient estimate

$$
|c_I|\leq\int_I|f(t)-f(x_I)||H_I(t)|\,dt\leq\omega_f(\ell)\sqrt\ell.
$$

In particular $|c_I|\leq2\|f\|_\infty\sqrt\ell$, so for every $\delta>0$ only finitely many details can have $|c_I|\geq\delta$. The hard-threshold sum

$$
T_\delta f=\sum_{|c_H|\geq\delta}c_HH
$$

is thus a well-defined finite sum. Its chosen details need not form a complete set of levels; this is why convergence of the [Haar projections](../../../fourier-analysis.md#haar-projection) alone does not prove the result.

Fix $\eta>0$. Choose $J\geq1$ so that $\omega_f(L2^{-J})\leq\eta$. All finer details satisfy $|c_I|\leq\eta\sqrt L\,2^{-j/2}$ at level $j\geq J$. For sufficiently small $\delta$, every nonzero coefficient at levels below $J$, and the constant coefficient if nonzero, is retained. Also choose the unique integer $K\geq J$ such that

$$
\frac{\delta2^{K/2}}{\sqrt L}\leq\eta<\frac{\delta2^{(K+1)/2}}{\sqrt L}.
$$

For $j>K$ we have $|c_I|\leq\eta\sqrt L2^{-j/2}<\delta$, so no such detail is retained. Consequently $T_\delta f$ differs from $A_{K+1}f$ only by omitted details at levels $J$ through $K$. At any point there is at most one supported detail per level, and an omitted detail has magnitude at most $\delta/\sqrt{L2^{-j}}$. The [geometric bound for omitted Haar details](../../../fourier-analysis.md#geometric-bound-for-omitted-haar-details) gives

$$
\|T_\delta f-A_{K+1}f\|_\infty\leq\sum_{j=J}^K\frac{\delta2^{j/2}}{\sqrt L}\leq\frac{\eta}{1-2^{-1/2}}.
$$

Since $\|A_{K+1}f-f\|_\infty\leq\eta$, we conclude

$$
\|T_\delta f-f\|_\infty\leq\left(1+\frac1{1-2^{-1/2}}\right)\eta.
$$

The right side can be made arbitrarily small, proving [uniform hard-threshold convergence of normalized Haar expansions](../../../fourier-analysis.md#uniform-hard-threshold-convergence-of-normalized-haar-expansions):

$$
\boxed{\left\|\sum_{|\widehat f(H)|\geq\delta}\widehat f(H)H-f\right\|_\infty\longrightarrow0\quad(\delta\downarrow0).}
$$

The square-root scaling imposed by the specified $L^2$ normalization is what makes the omitted contributions a controlled [geometric series](../../../real-analysis.md#geometric-series).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
