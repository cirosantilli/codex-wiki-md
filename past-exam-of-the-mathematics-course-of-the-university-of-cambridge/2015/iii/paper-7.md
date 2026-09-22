# Paper 7

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_7.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_7.pdf)

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

## 1

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Consider the operators on all of $C_0(X)$ or $L^2(\mu)$, extending the displayed positive-function formula linearly. Here $C_0(X)$ is the [space of continuous functions vanishing at infinity](../../../functional-analysis.md#space-of-continuous-functions-vanishing-at-infinity). The multiplier has modulus at most one, so $\|P_tf\|\leq\|f\|$, and multiplication of exponentials gives $P_{s+t}=P_sP_t$ and $P_0=I$. For [strong continuity](../../../functional-analysis.md#strong-continuity) on $C_0(X)$, choose a compact $K$ outside which $|f|$ is small. On $K$ the continuous $k$ is bounded, making $e^{-tk}\to1$ uniform; outside $K$, $|(e^{-tk}-1)f|\leq|f|$. For $L^2(\mu)$, use [pointwise convergence](../../../real-analysis.md#pointwise-convergence) and the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) with bound $|(e^{-tk}-1)f|^2\leq|f|^2$. Thus both are [contraction semigroups](../../../functional-analysis.md#contraction-semigroup), even when $k$ is unbounded.

The [generator of a multiplication semigroup](../../../functional-analysis.md#generator-of-a-multiplication-semigroup) is

$$
\boxed{Lf=-kf,\qquad D_{C_0}(L)=\{f\in C_0(X):kf\in C_0(X)\},\qquad D_2(L)=\{f\in L^2(\mu):kf\in L^2(\mu)\}.}
$$

Indeed pointwise difference quotients converge to $-kf$. A [norm](../../../functional-analysis.md#norm) limit therefore forces the displayed domain condition, using an almost-everywhere convergent subsequence for the $L^2$ case. Conversely $|(e^{-tk}-1)/t|\leq k$, so the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) proves the $L^2$ limit when $kf\in L^2$. In $C_0(X)$ write the error as $kf$ times $1-(1-e^{-tk})/(tk)$, with the value at $k=0$ supplied by continuity. That second factor tends uniformly to zero where $k$ is bounded and has modulus at most one; the compact-set and small-tail argument applied to $kf$ proves [uniform convergence](../../../real-analysis.md#uniform-convergence). To prove directly that $L$ is a [closed operator](../../../functional-analysis.md#closed-linear-operator), take $f_n\to f$ and $Lf_n\to g$. Pointwise limits in $C_0$, or a common almost-everywhere convergent subsequence in $L^2$, give $g=-kf$. Thus $f$ is in the appropriate [generator domain](../../../functional-analysis.md#generator-domain) and $Lf=g$. In $L^2$ the domain is dense because $f\mathbf1_{\{k\leq n\}}\to f$; in $C_0$ compactly supported [continuous functions](../../../calculus.md#continuous-function) are a dense subspace contained in the domain.

A real [multiplication operator](../../../vector-space.md#multiplication-operator) on its maximal $L^2$ domain is an [unbounded self-adjoint operator](../../../linear-operator-theory.md#unbounded-self-adjoint-operator). One direct verification is to test the adjoint relation against functions supported on $\{k\leq n\}$. If $h$ is in the [adjoint operator](../../../hilbert-space.md#adjoint-operator) domain with representing vector $g$, those tests force $g=-kh$ on each such set, hence $kh\in L^2$. The converse follows by integration. On the [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) spaces used below, the [spectrum of a real multiplication operator](../../../vector-space.md#spectrum-of-a-real-multiplication-operator) is its [essential range](../../../measure-theory.md#essential-range); spectral values are detected by [unit vectors](../../../vector-space.md#unit-vector) supported where the multiplier is arbitrarily close to that value, while outside the essential range its reciprocal is a bounded resolvent multiplier.

For the [heat semigroup](../../../diffusion-equation.md#heat-semigroup) on $L^2(\mathbb R,dx)$, take the normalization $L_H=f''$. The unitary [Fourier transform](../../../analysis.md#fourier-transform) converts it to multiplication by $-\xi^2$, and converts the semigroup to multiplication by $e^{-t\xi^2}$. Consequently

$$
\boxed{D(L_H)=H^2(\mathbb R),\qquad\sigma(L_H)=(-\infty,0],\qquad L_H=L_H^*.}
$$

The [Sobolev space](../../../sobolev-space.md) domain is exactly $\{f:\xi^2\widehat f\in L^2\}$. The continuous [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis) comes from the full [essential range](../../../measure-theory.md#essential-range) of $-\xi^2$, not from square-integrable Fourier [eigenvectors](../../../linear-operator-theory.md#eigenvector).

For the [Ornstein-Uhlenbeck semigroup](../../../functional-analysis.md#ornstein-uhlenbeck-semigroup) on standard [Gaussian measure](../../../stochastic-process.md#gaussian-measure), the normalized [Probabilists' Hermite polynomials](../../../numerical-analysis.md#probabilists-hermite-polynomial) $h_n=\operatorname{He}_n/\sqrt{n!}$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). The construction below gives $L_{OU}=D^2-xD$ and $L_{OU}h_n=-nh_n$, so the Hermite coefficient map turns it into a real [multiplication operator](../../../vector-space.md#multiplication-operator) on $\ell^2(\mathbb N_0)$. Therefore

$$
\boxed{D(L_{OU})=\left\{\sum_{n\geq0}c_nh_n:\sum_{n\geq0}n^2|c_n|^2<\infty\right\},\quad\sigma(L_{OU})=\{0,-1,-2,\ldots\},\quad L_{OU}=L_{OU}^*.}
$$

Finally, **the heat semigroup on the whole real line has no positive [spectral gap](../../../linear-operator-theory.md#spectral-gap)**, whereas **the standard [Ornstein-Uhlenbeck semigroup](../../../functional-analysis.md#ornstein-uhlenbeck-semigroup) has gap one**. For the first claim, take a nonzero smooth compactly supported $\phi$ and set $f_R(x)=R^{-1/2}\phi(x/R)$. Then $\|f_R\|_2^2=\|\phi\|_2^2$, but $\|f_R'\|_2^2=R^{-2}\|\phi'\|_2^2$. This disproves a uniform whole-line [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) $\|f\|_2^2\leq C\|f'\|_2^2$; one can also choose $\int\phi=0$. Lebesgue measure here is infinite, so it has no normalized probability mean to subtract. For [Gaussian measure](../../../stochastic-process.md#gaussian-measure), the Hermite expansion instead gives the sharp [Gaussian Poincaré inequality](../../../probability-inequality.md#gaussian-poincare-inequality)

$$
\boxed{\operatorname{Var}_\gamma(f)=\sum_{n\geq1}|c_n|^2\leq\sum_{n\geq1}n|c_n|^2=\int|f'|^2\,d\gamma.}
$$

Equality holds for affine functions. The identity on the right is interpreted on the energy-form domain, which is larger than the full [operator domain](../../../vector-space.md#operator-domain).

## 2

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

On a compact [metric space](../../../topological-analysis.md#metric-space) $X$, a conservative [Feller semigroup](../../../functional-analysis.md#feller-semigroup) is a [strongly continuous semigroup](../../../functional-analysis.md#c0-semigroup) of positive linear maps on $C(X)$ satisfying $P_t1=1$. [Positivity](../../../quantum-information-theory.md#positivity-linear-maps) means $f\geq0\Longrightarrow P_tf\geq0$. These conditions imply sup-norm contraction. Conversely, for a [contraction semigroup](../../../functional-analysis.md#contraction-semigroup) with $1\in D(L)$ and $L1=0$, differentiation on the [generator domain](../../../functional-analysis.md#generator-domain) gives $\frac{d}{dt}P_t1=P_tL1=0$, so $P_t1=1$. On the real space $C(X)$, if $0\leq f\leq1$, then $\|1-P_tf\|_\infty\leq\|1-f\|_\infty\leq1$, implying $P_tf\geq0$. Scaling proves [positivity](../../../quantum-information-theory.md#positivity-linear-maps) for every nonnegative $f$. This is the [unital contraction positivity criterion](../../../continuous-dual-space.md#unital-contraction-positivity-criterion). For complex $C(X)$ the same conclusion follows because each functional $f\mapsto P_tf(x)$ has [norm](../../../functional-analysis.md#norm) one and value one on $1$, hence is a [positive linear functional](../../../continuous-dual-space.md#positive-linear-functional).

For each $t,x$, the [Riesz-Markov-Kakutani representation theorem](../../../functional-analysis.md#riesz-markov-kakutani-representation-theorem) represents that functional by a unique [Borel probability measure](../../../measure-theory.md#borel-probability-measure) $p_t(x,dy)$:

$$
\boxed{P_tf(x)=\int_X f(y)\,p_t(x,dy).}
$$

Continuity of $P_tf$ gives weak continuity of $x\mapsto p_t(x,\cdot)$. Approximating indicators of open sets increasingly by [continuous functions](../../../calculus.md#continuous-function) proves Borel measurability in $x$; a monotone-class argument then gives a [Markov kernel](../../../markov-process.md#markov-kernel). The [semigroup property](../../../functional-analysis.md#semigroup-property) and uniqueness of representing measures yield $p_0(x,\cdot)=\delta_x$ and the [Chapman-Kolmogorov equation](../../../markov-process.md#chapman-kolmogorov-equation)

$$
p_{s+t}(x,A)=\int_X p_t(y,A)\,p_s(x,dy).
$$

These are the required [transition probabilities](../../../markov-process.md#transition-probability).

An [invariant probability measure for a semigroup](../../../measure-theory.md#invariant-probability-measure-for-a-semigroup) satisfies $\int_XP_tf\,d\mu=\int_Xf\,d\mu$ for every $t\geq0$ and $f\in C(X)$. Equivalently its distribution is preserved by the [Markov kernel](../../../markov-process.md#markov-kernel). For $1\leq p<\infty$, [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives $|P_tf|^p\leq P_t(|f|^p)$ pointwise. Integrating and using invariance proves

$$
\boxed{\|P_tf\|_{L^p(\mu)}\leq\|f\|_{L^p(\mu)}.}
$$

Also $\|P_tf-f\|_{L^p(\mu)}\leq\|P_tf-f\|_\infty\to0$. [Continuous functions](../../../calculus.md#continuous-function) are dense in these $L^p$ spaces for a finite [Borel measure](../../../measure-theory.md#borel-measure) on a compact metric space, so the contraction extends to a [strongly continuous semigroup](../../../functional-analysis.md#c0-semigroup) on $L^p(\mu)$.

For real $f$ with $f,f^2\in D(L)$, the kernel form of [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives $P_t(f^2)-(P_tf)^2\geq0$, with equality at $t=0$. Take its right [derivative](../../../calculus.md#derivative) to obtain the [generator square inequality](../../../functional-analysis.md#generator-square-inequality)

$$
\boxed{L(f^2)\geq2fLf.}
$$

This is nonnegativity of the associated [carré du champ](../../../functional-analysis.md#carre-du-champ-operator).

Each time-average functional $\phi_n$ is positive with $\phi_n(1)=1$, hence represents a [Borel probability measure](../../../measure-theory.md#borel-probability-measure) $\mu_n$. The [compactness of probability measures on a compact metric space](../../../convergence-of-random-variables.md#compactness-of-probability-measures-on-a-compact-metric-space) gives a subsequence converging weakly to a probability measure $\mu$. Explicitly, $C(X)$ is a [separable Banach space](../../../banach-space.md#separable-banach-space), so [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) and a countable dense family give a subsequence converging on every [continuous function](../../../calculus.md#continuous-function), rather than merely a net. For fixed $t\geq0$, the [semigroup property](../../../functional-analysis.md#semigroup-property) gives the [Krylov-Bogolyubov time-average argument](../../../measure-theory.md#krylov-bogolyubov-theorem):

$$
\phi_n(P_tf)-\phi_n(f)=\frac1n\left[\int_n^{n+t}\!\int_XP_sf\,d\nu\,ds-\int_0^t\!\int_XP_sf\,d\nu\,ds\right].
$$

Its absolute value is at most $2t\|f\|_\infty/n$. Pass to the subsequential limit, observing that $P_tf\in C(X)$, to get $\int_XP_tf\,d\mu=\int_Xf\,d\mu$. Thus the limiting measure is invariant.

## 3

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a densely defined operator $A$ on a complex [Hilbert space](../../../hilbert-space.md), [unbounded self-adjointness](../../../linear-operator-theory.md#unbounded-self-adjoint-operator) means equality $A=A^*$ including equality of the [operator domains](../../../vector-space.md#operator-domain). Symmetry alone asserts only $A\subseteq A^*$ and is insufficient. Use an [inner product](../../../linear-algebra.md#inner-product) linear in its first argument. If $\operatorname{Im}z\ne0$, symmetry gives

$$
\|(A-z)u\|\,\|u\|\geq|\operatorname{Im}\langle(A-z)u,u\rangle|=|\operatorname{Im}z|\|u\|^2.
$$

Thus $A-z$ is bounded below. Since $A$ is closed, its range is closed; its orthogonal complement is $\ker(A^*-\overline z)=\ker(A-\overline z)=0$, so the range is also dense and therefore all of $H$. The inverse is bounded by $|\operatorname{Im}z|^{-1}$. The [nonreal resolvent estimate for a self-adjoint operator](../../../linear-operator-theory.md#nonreal-resolvent-estimate-for-a-self-adjoint-operator) proves **$\sigma(A)\subseteq\mathbb R$**.

For bounded [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) $T$, its [numerical range of an operator](../../../functional-analysis.md#numerical-range-of-an-operator) and [numerical radius](../../../functional-analysis.md#numerical-radius) are

$$
W(T)=\{\langle Tu,u\rangle:\|u\|=1\},\qquad w(T)=\sup_{\|u\|=1}|\langle Tu,u\rangle|.
$$

Every number in $W(T)$ is real. If $z\notin\overline{W(T)}$, its distance $\delta$ from that closed set is positive, and $\|(T-z)u\|\geq\delta\|u\|$. The same bound applies to $T-\overline z$, so the range is dense as well as closed and $T-z$ has a bounded inverse. Hence the [numerical-range spectral enclosure](../../../functional-analysis.md#numerical-range-spectral-enclosure) is

$$
\boxed{\sigma(T)\subseteq\overline{W(T)}\subseteq\mathbb R.}
$$

The closure is necessary in infinite dimension: the endpoints of the numerical range need not themselves be attained.

Put $\beta=\sup W(T)$ and $B=\beta I-T$, a bounded [positive semidefinite operator](../../../hilbert-space.md#positive-operator). Choose [unit vectors](../../../vector-space.md#unit-vector) $u_n$ with $\langle Bu_n,u_n\rangle\to0$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for the positive form $\langle B\cdot,\cdot\rangle$ implies

$$
\|Bu_n\|^2=\sup_{\|v\|=1}|\langle Bu_n,v\rangle|^2\leq\|B\|\langle Bu_n,u_n\rangle\longrightarrow0.
$$

Therefore $\beta$ is an [approximate eigenvalue](../../../linear-operator-theory.md#approximate-eigenvalue). Apply the same argument to $T-\alpha I$, where $\alpha=\inf W(T)$, to get the other endpoint. This proves the [numerical-range endpoint approximate-eigenvalue theorem](../../../functional-analysis.md#numerical-range-endpoint-approximate-eigenvalue-theorem). Each endpoint is in the [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis): a bounded inverse would forbid [unit vectors](../../../vector-space.md#unit-vector) with vanishing residual.

If an [unbounded self-adjoint operator](../../../linear-operator-theory.md#unbounded-self-adjoint-operator) $A$ is positive semidefinite, then for every real $z<0$, $\|(A-z)u\|\geq(-z)\|u\|$. The range argument above again proves invertibility, excluding negative values from the [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis). For the converse, suppose $\sigma(A)\subseteq[0,\infty)$. Its [resolvent operator](../../../functional-analysis.md#resolvent-of-an-operator) $R=(I+A)^{-1}$ is bounded and self-adjoint. The [resolvent spectral mapping identity](../../../mathematics.md#resolvent-spectral-mapping-identity) puts $\sigma(R)\subseteq[0,1]$: for $w\ne0$, the relevant spectral parameter of $A$ is $1/w-1$, and nonreal values are excluded by self-adjointness. By the endpoint result just proved, $W(R)\subseteq[0,1]$. Positive-form [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) then gives

$$
\|Rf\|^2\leq\langle Rf,f\rangle\sup_{\|v\|=1}\langle Rv,v\rangle\leq\langle Rf,f\rangle.
$$

For $u=Rf\in D(A)$ this yields $\langle Au,u\rangle=\langle f-Rf,Rf\rangle\geq0$. Thus the [spectral positivity criterion for a self-adjoint operator](../../../linear-operator-theory.md#spectral-positivity-criterion-for-a-self-adjoint-operator) is

$$
\boxed{A\geq0\quad\Longleftrightarrow\quad\sigma(A)\subseteq[0,\infty).}
$$

This resolvent proof uses the bounded numerical-range result to handle the full unbounded domain.

## 4

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Identify $G$ with the [Boolean hypercube](../../../combinatorics.md#boolean-hypercube) $\{-1,1\}^d$, with coordinatewise multiplication and normalized [Haar measure](../../../measure-theory.md#haar-measure) assigning mass $2^{-d}$ to each point. Its [Bernoulli function](../../../probability-theory.md#bernoulli-function-hypercube) $\epsilon_i(\omega)=\omega_i$ is a [Rademacher random variable](../../../probability-theory.md#rademacher-distribution). The [Walsh functions on a hypercube](../../../combinatorics.md#walsh-character) are the [Walsh characters](../../../combinatorics.md#walsh-character) $w_A=\prod_{i\in A}\epsilon_i$, indexed by all subsets $A\subseteq\{1,\ldots,d\}$, including $w_\varnothing=1$. Independence of the sign coordinates gives $\langle w_A,w_B\rangle=\mathbb E w_{A\triangle B}=\mathbf1_{A=B}$. There are $2^d$ characters, equal to the dimension of $L^2(G)$, so they form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis).

Flipping coordinate $i$ negates $w_A$ exactly when $i\in A$. Thus the [coordinate-flip generator on a hypercube](../../../combinatorics.md#coordinate-flip-generator-on-a-hypercube) satisfies

$$
\boxed{Lw_A=-|A|w_A,\qquad\sigma(L)=\{0,-1,\ldots,-d\},\qquad\text{multiplicity of }-j=\binom dj.}
$$

For $f=\sum_A\widehat f(A)w_A$, [Parseval identity](../../../fourier-analysis.md#parseval-identity) gives $\langle f,Lf\rangle=-\sum_A|A||\widehat f(A)|^2\leq0$. Equivalently its [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) is

$$
\mathcal E(f)=-\mathbb E[fLf]=\frac14\sum_{i=1}^d\mathbb E\bigl(f(\omega^{(i)})-f(\omega)\bigr)^2,
$$

where $\omega^{(i)}$ flips coordinate $i$.

Set $S(\omega)=\sum_i a_i\epsilon_i(\omega)$ and $F(\omega)=\|S(\omega)\|$. Since $F(-\omega)=F(\omega)$, its Walsh expansion contains only sets $A$ of even size. Every nonconstant such set has $|A|\geq2$, giving the [even-function spectral gap on a hypercube](../../../combinatorics.md#even-function-spectral-gap-on-a-hypercube)

$$
2\operatorname{Var}(F)\leq\mathcal E(F).
$$

At each $S(\omega)$ the [Hahn-Banach theorem](../../../functional-analysis.md#hahn-banach-theorem) supplies a real supporting linear functional $\ell$ of [norm](../../../functional-analysis.md#norm) at most one with $\ell(S)=\|S\|$; for a complex normed space use the real part of a complex norming functional. At $S=0$ take $\ell=0$. Convexity of the [norm](../../../functional-analysis.md#norm) gives $F(\omega^{(i)})-F(\omega)\geq\ell(S(\omega^{(i)})-S(\omega))$. Since $LS=-S$, sum these inequalities to get $LF\geq-F$. Therefore $\mathcal E(F)=-\mathbb E[FLF]\leq\mathbb EF^2$. Combining the two bounds yields the [sharp Rademacher second-moment inequality](../../../fourier-analysis.md#sharp-rademacher-second-moment-inequality)

$$
\boxed{\mathbb E\left\|\sum_i a_i\epsilon_i\right\|^2\leq2\left(\mathbb E\left\|\sum_i a_i\epsilon_i\right\|\right)^2.}
$$

No smoothness of the [norm](../../../functional-analysis.md#norm) is required. The constant $2$ is sharp: two equal nonzero real coefficients give modulus $0$ or $2|a|$ with equal probabilities. This is the second-versus-first moment case of the [Kahane-Khintchine inequality](../../../fourier-analysis.md#kahane-khintchine-inequality) for arbitrary [normed vector spaces](../../../functional-analysis.md#normed-vector-space).

For the complex-circle assertion, write each independent [Steinhaus random variable](../../../continuous-probability-distribution.md#steinhaus-random-variable) as $\eta_i=\epsilon_i\cos\theta_i+i\delta_i\sin\theta_i$, where $\theta_i$ is uniform on $[0,\pi/2]$ and all quadrant signs $\epsilon_i,\delta_i$ are independent. Conditional on the angles, $\sum_i a_i\eta_i$ is a [Rademacher sum](../../../probability-theory.md#rademacher-sum) with $2d$ complex coefficients $a_i\cos\theta_i$ and $ia_i\sin\theta_i$. Its conditional second moment is $\sum_i|a_i|^2$, independent of the angles. The preceding inequality gives its conditional first moment at least $\sqrt{\frac12\sum_i|a_i|^2}$. Average over the angles and square to obtain the [Steinhaus first-moment lower bound](../../../continuous-probability-distribution.md#steinhaus-first-moment-lower-bound)

$$
\boxed{\sum_i|a_i|^2\leq2\left(\mathbb E\left|\sum_i a_i\eta_i\right|\right)^2.}
$$

## 5

↑ **Parent:** [Paper 7](paper-7.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

On the polynomial subspace of $L^2(\gamma)$, the [Gaussian creation and annihilation operators](../../../functional-analysis.md#gaussian-creation-and-annihilation-operators) are $a^-=D$ and $a^+=x-D$. [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) makes them adjoints there and gives $[a^-,a^+]=I$. The [Gaussian number operator](../../../functional-analysis.md#gaussian-number-operator) is

$$
\boxed{N=a^+a^-=-D^2+xD.}
$$

The [Probabilists' Hermite polynomials](../../../numerical-analysis.md#probabilists-hermite-polynomial) are $\operatorname{He}_n(x)=(-1)^ne^{x^2/2}D^ne^{-x^2/2}=(a^+)^n1$. Their generating function is $e^{sx-s^2/2}=\sum_n\operatorname{He}_n(x)s^n/n!$, giving $D\operatorname{He}_n=n\operatorname{He}_{n-1}$. The commutator also yields

$$
\boxed{N\operatorname{He}_n=n\operatorname{He}_n,\qquad\int\operatorname{He}_m\operatorname{He}_n\,d\gamma=n!\,\mathbf1_{m=n}.}
$$

The orthogonality follows by repeated [integration by parts](../../../calculus.md#integration-by-parts); the leading coefficient is one, so these polynomials span every polynomial. By the allowed density assumption $h_n=\operatorname{He}_n/\sqrt{n!}$ is an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Define the closed number operator by $N\sum c_nh_n=\sum nc_nh_n$ on $\sum n^2|c_n|^2<\infty$. This diagonal [multiplication operator](../../../vector-space.md#multiplication-operator) is self-adjoint and positive semidefinite; polynomial truncations show it is the closure of the polynomial operator.

The [Ornstein-Uhlenbeck semigroup](../../../functional-analysis.md#ornstein-uhlenbeck-semigroup) is $P_t=e^{-tN}$, or $P_tf=\sum_ne^{-nt}c_nh_n$. It also has the [Mehler formula for the Ornstein-Uhlenbeck semigroup](../../../functional-analysis.md#mehler-formula-for-the-ornstein-uhlenbeck-semigroup)

$$
\boxed{P_tf(x)=\mathbb E\left[f\!\left(e^{-t}x+\sqrt{1-e^{-2t}}\,Z\right)\right],\qquad Z\sim N(0,1).}
$$

To verify the formula, apply its right side to $e^{sx-s^2/2}$: the [Gaussian moment-generating function](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) makes the result $e^{se^{-t}x-s^2e^{-2t}/2}$, proving the [eigenvalue](../../../linear-operator-theory.md#eigenvalue) identity on every Hermite polynomial. [Positivity](../../../quantum-information-theory.md#positivity-linear-maps) and invariance of [Gaussian measure](../../../stochastic-process.md#gaussian-measure) give $L^2$ contraction by [Jensen inequality](../../../real-analysis.md#jensen-s-inequality), so polynomial density extends the equality to all $L^2(\gamma)$. The coefficient expansion gives

$$
\|P_tf-\mathbb E_\gamma f\|_2^2=\sum_{n\geq1}e^{-2nt}|c_n|^2\longrightarrow0.
$$

For continuously differentiable $f$ with bounded [derivative](../../../calculus.md#derivative), differentiate the Mehler expectation by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) to get the [Ornstein-Uhlenbeck gradient commutation identity](../../../functional-analysis.md#ornstein-uhlenbeck-gradient-commutation-identity)

$$
\boxed{(P_tf)'=e^{-t}P_t(f').}
$$

The same identity extends to the [Gaussian Sobolev form domain](../../../sobolev-space.md#gaussian-sobolev-space). Mehler's formula also gives [pointwise convergence](../../../real-analysis.md#pointwise-convergence) to the Gaussian mean for such $f$, since bounded [derivative](../../../calculus.md#derivative) permits at most linear growth.

The [Gaussian Dirichlet energy](../../../functional-analysis.md#gaussian-dirichlet-energy) is the energy form of $N$:

$$
\boxed{\mathcal E_\gamma(f)=\lim_{t\downarrow0}\frac{\|f\|_2^2-\langle f,P_tf\rangle}{t}=\sum_{n\geq1}n|c_n|^2=\int|f'|^2\,d\gamma.}
$$

For polynomials this follows from $N=(a^-)^*a^-$, and closure extends it to the form domain. For the given continuously differentiable $f$, [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) yields $\langle f',h_{n-1}\rangle=\sqrt n c_n$, so [Parseval identity](../../../fourier-analysis.md#parseval-identity) proves the derivative-energy equality directly. Bounded [derivative](../../../calculus.md#derivative) puts $f$ in the [Gaussian Sobolev space](../../../sobolev-space.md#gaussian-sobolev-space), hence in that form domain; it need not be in the full [operator domain](../../../vector-space.md#operator-domain), so $\langle f,Nf\rangle$ is not always a legitimate initial definition.

Use the [entropy functional](../../../probability-inequality.md#entropy-functional) $\operatorname{Ent}_\gamma(h)=\int h\log h\,d\gamma-(\int h\,d\gamma)\log\int h\,d\gamma$. Begin with bounded smooth $h>0$ bounded away from zero, and put $h_t=P_th$. Invariance and [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) give the [Ornstein-Uhlenbeck entropy dissipation identity](../../../probability-inequality.md#ornstein-uhlenbeck-entropy-dissipation-identity)

$$
-\frac{d}{dt}\operatorname{Ent}_\gamma(h_t)=\int\frac{|h_t'|^2}{h_t}\,d\gamma.
$$

The gradient identity and the permitted weighted [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), applied with weight $h$, imply

$$
\frac{|h_t'|^2}{h_t}=e^{-2t}\frac{|P_t(h')|^2}{P_th}\leq e^{-2t}P_t\!\left(\frac{|h'|^2}{h}\right).
$$

The entropy tends to zero as $t\to\infty$ by Mehler's formula and bounded convergence. Integrating in time and using invariance yields $\operatorname{Ent}_\gamma(h)\leq\frac12\int|h'|^2/h\,d\gamma$. Set $h=f^2$ to obtain the sharp [Gaussian logarithmic Sobolev inequality](../../../probability-inequality.md#gaussian-logarithmic-sobolev-inequality)

$$
\boxed{\operatorname{Ent}_\gamma(f^2)\leq2\int|f'|^2\,d\gamma=2\mathcal E_\gamma(f).}
$$

For the stated possibly unbounded $f$, apply the argument to smooth positive clipped approximations with a common positive lower bound and uniformly bounded [derivatives](../../../calculus.md#derivative). They can converge pointwise together with their [derivatives](../../../calculus.md#derivative) and have a common linear-growth bound. Since [Gaussian measure](../../../stochastic-process.md#gaussian-measure) integrates every polynomial moment, [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) passes both the entropy and the [derivative](../../../calculus.md#derivative) energy to the limit. This also justifies use of the supplied inequality when $2ff'$ itself is unbounded. The normalization $\|f\|_1=1$ concerns $f$, and does not imply $\int f^2\,d\gamma=1$; the second term in the entropy definition must be retained.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
