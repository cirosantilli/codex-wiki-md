# Paper 216

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_216.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_216.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [likelihood function](../../../statistical-modelling.md#likelihood-function) and [prior distribution](../../../statistical-inference.md#prior-probability) give the [posterior density](../../../statistical-inference.md#posterior-density)

$$
\pi(\beta\mid Y)\propto
\exp\left\{-\frac12(Y-X\beta)^T\Sigma_e^{-1}(Y-X\beta)
-\frac12\beta^T\Sigma^{-1}\beta\right\}.
$$

Completing the square in the [quadratic form](../../../linear-algebra.md#quadratic-form) gives

$$
C=\left(X^T\Sigma_e^{-1}X+\Sigma^{-1}\right)^{-1},
\qquad
m=CX^T\Sigma_e^{-1}Y.
$$

Thus [Gaussian conjugacy for a normal linear model](../../../statistical-modelling.md#gaussian-conjugacy-for-a-normal-linear-model) yields

$$
\boxed{\beta\mid Y\sim N(m,C).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

After integrating out the [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) $\beta$, the [marginal distribution](../../../probability-theory.md#marginal-distribution) is

$$
Y\sim N\!\left(0,\sigma^2A\right),
\qquad A=XX^T+\alpha I_n.
$$

Up to terms independent of $\sigma^2$, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\sigma^2)=-\frac n2\log\sigma^2
-\frac1{2\sigma^2}Y^TA^{-1}Y.
$$

Differentiating and setting the result to zero gives the [maximum marginal likelihood estimator](../../../statistical-inference.md#maximum-marginal-likelihood-estimator)

$$
\widehat{\sigma}^2=\frac1nY^T(XX^T+\alpha I_n)^{-1}Y.
$$

This is an [Empirical Bayes method](../../../statistical-inference.md#empirical-bayes-method) because the estimated [hyperparameter](../../../statistical-inference.md#hyperparameter) is then inserted into the prior and posterior distributions.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a decision $x$ in the [unit ball](../../../functional-analysis.md#unit-ball), [conditional expectation](../../../measure-theory.md#conditional-expectation) under the posterior gives

$$
\mathbb E[(x^T\beta)^2\mid Y]
=x^T\mathbb E[\beta\beta^T\mid Y]x
=x^T(C+mm^T)x.
$$

The symmetric [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) $C+mm^T$ has a [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) maximized over $\lVert x\rVert\leq1$ by any unit [eigenvector](../../../linear-operator-theory.md#eigenvector) corresponding to its largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue). [Bayes decision rule](../../../statistical-inference.md#bayes-decision-rule) therefore chooses any such eigenvector for the stated utility.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For the first $i$ observations, write

$$
A_i=\Sigma^{-1}+X_{1:i}^TX_{1:i},
\qquad b_i=X_{1:i}^TY_{1:i}.
$$

By [Gaussian conjugacy for a normal linear model](../../../statistical-modelling.md#gaussian-conjugacy-for-a-normal-linear-model), the prefix posterior is

$$
\beta\mid Y_{1:i}\sim N(A_i^{-1}b_i,A_i^{-1}).
$$

Compute a [Cholesky decomposition](../../../linear-algebra.md#cholesky-decomposition) of $A_0=\Sigma^{-1}$ once. If $x_i^T$ is row $i$ of the [design matrix](../../../linear-regression.md#design-matrix), then

$$
A_i=A_{i-1}+x_ix_i^T,
\qquad b_i=b_{i-1}+x_iY_i.
$$

The [Rank-one Cholesky update](../../../linear-algebra.md#rank-one-cholesky-update) obtains a triangular factor $A_i=L_iL_i^T$ from $L_{i-1}$ in $O(p^2)$ operations. Two [triangular solves](../../../linear-algebra.md#triangular-linear-system) give $m_i=A_i^{-1}b_i$, and, for $z_i\sim N(0,I_p)$, another solve gives

$$
\beta_i=m_i+L_i^{-T}z_i\sim N(m_i,A_i^{-1}).
$$

The initial factorization costs $O(p^3)$ and all $n$ updates and samples cost $O(np^2)$. This is within the requested $O(p^3+np^2+n^2p)$ bound.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Put $z_i=\log Y_i$. The [Weighted graph Laplacian](../../../graph-theory.md#weighted-graph-laplacian) $L_J$ of the tree is defined by

$$
\beta^TL_J\beta
=\sum_{i\ne v_0}J_i(\beta_i-\beta_{a(i)})^2.
$$

Multiplication of the [Gaussian likelihood](../../../statistical-modelling.md#gaussian-likelihood) by the prior shows that, conditionally on the [precision parameter](../../../statistical-modelling.md#precision-parameter) $\tau$,

$$
\pi(\beta\mid Y,\tau)
\propto\exp\left\{-\frac12\beta^TM\beta
+\tau z^T\beta\right\},
\qquad
M=\tau I+2L_J+2cI.
$$

Completing the square therefore gives

$$
\beta\mid Y,\tau\sim N(M^{-1}\tau z,M^{-1}).
$$

As a function of $\tau$, the posterior density is

$$
\tau^{n/2}\exp\left\{-\tau\left(1+\frac12\lVert z-\beta\rVert^2\right)\right\},
$$

so, in shape-rate notation,

$$
\tau\mid Y,\beta\sim
\operatorname{Gamma}\left(\frac n2+1,
1+\frac12\lVert z-\beta\rVert^2\right).
$$

The [precision matrix](../../../variance.md#precision-matrix) $M$ has the [sparsity pattern](../../../vector-space.md#sparse-matrix) of a [tree](../../../combinatorics.md#tree-graph-theory). A sparse [Cholesky decomposition](../../../linear-algebra.md#cholesky-decomposition) and its triangular solves have $O(n)$ cost and storage on this graph, while the gamma update also costs $O(n)$. Hence each systematic-scan [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) iteration costs $O(n)$.

## 2

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [Markov kernel](../../../markov-process.md#markov-kernel) $K$ with [stationary distribution](../../../markov-process.md#stationary-distribution) $\pi$ is [geometrically ergodic](../../../statistical-inference.md#geometric-ergodicity) if there are $\rho<1$ and a finite function $M(x)$ such that

$$
\lVert K^m(x,\mathord\cdot)-\pi\rVert_{\mathrm{TV}}
\leq M(x)\rho^m
$$

for every $m\geq0$ and almost every starting point $x$, where $\lVert\cdot\rVert_{\mathrm{TV}}$ is [total variation distance](../../../probability-and-statistics.md#total-variation-distance).

A measurable set $A$ is a [small set](../../../statistical-inference.md#small-set) with minorisation constant $\alpha>0$ if some integer $r\geq1$ and some [probability measure](../../../probability-theory.md#probability-measure) $\nu$ satisfy

$$
K^r(x,B)\geq\alpha\nu(B)
$$

for every $x\in A$ and every measurable $B$.

A standard [drift-minorisation condition](../../../statistical-inference.md#drift-minorisation-condition) is that the chain be [irreducible](../../../markov-process.md#irreducible-markov-chain) and [aperiodic](../../../markov-process.md#aperiodic-markov-chain), and that there exist a measurable $V\geq1$, a small set $A$, constants $\lambda<1$ and $b<\infty$ such that

$$
KV(x)\leq\lambda V(x)+b\mathbf1_A(x).
$$

These conditions imply geometric ergodicity.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Multiplying the [exponential family](../../../exponential-family.md) likelihood by its [natural conjugate prior](../../../exponential-family.md#natural-conjugate-prior) gives

$$
\pi(\theta\mid x)
=\exp\left\{
\theta^T(\lambda_1+T(x))
-Z(\theta)(\lambda_2+1)
-\widetilde Z(\lambda_1+T(x),\lambda_2+1)
\right\}.
$$

Thus the posterior remains in the same family, with updated [hyperparameters](../../../statistical-inference.md#hyperparameter)

$$
\lambda_1'=\lambda_1+T(x),
\qquad \lambda_2'=\lambda_2+1.
$$

Under [quadratic loss](../../../statistical-inference.md#squared-error-loss), the [Bayes estimator under squared error loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss) is the [posterior mean](../../../statistical-inference.md#posterior-mean). Differentiating the [log-partition function](../../../exponential-family.md#cumulant-function-of-an-exponential-family) that normalizes the conjugate prior gives

$$
\boxed{\widehat\theta
=\mathbb E[\theta\mid x]
=\nabla_{\lambda_1}\widetilde Z
(\lambda_1+T(x),\lambda_2+1).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $w(\theta)=\pi(\theta)/\mu(\theta)$ be the [importance weight](../../../probability-and-statistics.md#importance-weight). The two normalized densities give

$$
\log w(\theta)
=-\lambda_2\{Z(\theta)-F(\theta)\}
-\widetilde Z(\lambda)+\widetilde F(\lambda).
$$

Since $|F-Z|<C$, there is a finite constant $M$ such that $w(\theta)\leq M$ everywhere. The [Independence Metropolis–Hastings algorithm](../../../statistical-inference.md#independence-metropolis-hastings-algorithm) has an accepted transition density satisfying

$$
\mu(y)\min\left\{1,\frac{w(y)}{w(x)}\right\}
\geq\frac1M\mu(y)w(y)
=\frac1M\pi(y).
$$

Consequently the whole state space is a [small set](../../../statistical-inference.md#small-set), with the one-step [minorization condition](../../../statistical-inference.md#minorization-condition) $K(x,\mathord\cdot)\geq M^{-1}\pi(\mathord\cdot)$. Iterating this [Doeblin condition](../../../statistical-inference.md#doeblin-s-condition) gives uniform geometric convergence in [total variation distance](../../../probability-and-statistics.md#total-variation-distance), so the chain is geometrically ergodic.

## 3

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Markov chain Monte Carlo asymptotic variance](../../../statistical-inference.md#markov-chain-monte-carlo-asymptotic-variance) for a stationary [Markov chain](../../../markov-process.md#markov-chain) and $\psi\in L^2(\pi)$ is

$$
\sigma_K^2(\psi)
=\lim_{n\to\infty}n\operatorname{Var}\left(
\frac1n\sum_{j=1}^n\psi(X_j)\right)
=\operatorname{Var}_\pi(\psi)
+2\sum_{k=1}^{\infty}
\operatorname{Cov}_\pi(\psi(X_0),\psi(X_k)),
$$

whenever the limit and series exist. If a [reversible Markov chain](../../../markov-process.md#reversible-markov-chain) has positive $L^2_0(\pi)$ [spectral gap](../../../linear-operator-theory.md#spectral-gap) $\gamma$, then the [spectral theorem for normal operators on a separable Hilbert space](../../../hilbert-space.md#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space) gives

$$
\boxed{\sigma_K^2(\psi)
\leq\left(\frac2\gamma-1\right)
\operatorname{Var}_\pi(\psi).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $f,g\in L^2(\pi)$, [detailed balance](../../../markov-process.md#detailed-balance) says that the measure $\pi(dx)K(x,dy)$ is invariant under exchanging $x$ and $y$. Therefore

$$
\begin{aligned}
\langle f,Kg\rangle_\pi
&=\int f(x)g(y)\,\pi(dx)K(x,dy)\\
&=\int f(y)g(x)\,\pi(dx)K(x,dy)
=\langle Kf,g\rangle_\pi.
\end{aligned}
$$

This is precisely the defining identity for a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

By the [stationary distribution](../../../markov-process.md#stationary-distribution) property, $X_1$ and $X_2$ have the same [marginal distribution](../../../probability-theory.md#marginal-distribution) $\pi$. Expanding the square gives

$$
\begin{aligned}
\frac12\mathbb E[(f(X_2)-f(X_1))^2]
&=\frac12\left(2\langle f,f\rangle_\pi
-2\mathbb E[f(X_1)f(X_2)]\right)\\
&=\langle f,f\rangle_\pi-\langle f,Kf\rangle_\pi\\
&=\langle f,(I-K)f\rangle_\pi
=\mathcal E_K(f).
\end{aligned}
$$

This is the probabilistic representation of the [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Subtracting the [expected value](../../../probability-theory.md#expected-value) of $f$ does not alter either side, so suppose $\pi(f)=0$. Since reversibility makes $K$ a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) and stationarity makes it a contraction,

$$
\mathcal E_{K^2}(f)
=\lVert f\rVert_{L^2(\pi)}^2-\lVert Kf\rVert_{L^2(\pi)}^2.
$$

The [Discrete-time Poincaré inequality for a Markov kernel](../../../statistical-inference.md#discrete-time-poincare-inequality-for-a-markov-kernel) is therefore equivalent to

$$
\lVert Kf\rVert_2^2
\leq\left(1-\frac1C\right)\lVert f\rVert_2^2.
$$

Applying this inequality successively to $f,Kf,\ldots,K^{t-1}f$ yields

$$
\operatorname{Var}_\pi(K^tf)
=\lVert K^tf\rVert_2^2
\leq\left(1-\frac1C\right)^t
\lVert f\rVert_2^2
=\left(1-\frac1C\right)^t\operatorname{Var}_\pi(f).
$$

Conversely, the asserted variance contraction with $t=1$ rearranges to the Poincaré inequality. Hence the two statements are equivalent.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Part c gives the integral representation

$$
\mathcal E_K(f)
=\frac12\int\pi(dx)K(x,dy)(f(y)-f(x))^2.
$$

The integrand vanishes on the diagonal $y=x$. Thus the assumed off-diagonal [Peskun ordering](../../../statistical-inference.md#peskun-ordering) implies

$$
\mathcal E_K(f)\geq\mathcal E_Q(f)
$$

for every $f\in L^2(\pi)$.

On the mean-zero subspace, the variational characterization of the [spectral gap](../../../linear-operator-theory.md#spectral-gap) of a positive reversible kernel is

$$
\operatorname{gap}(K)
=\inf_{\pi(f)=0,\ f\ne0}
\frac{\mathcal E_K(f)}{\operatorname{Var}_\pi(f)}.
$$

It follows immediately that

$$
\operatorname{gap}(K)\geq\operatorname{gap}(Q).
$$

Equivalently, the energy inequality says $K\preceq Q$ in the [Löwner order](../../../hilbert-space.md#lowner-order) on $L^2_0(\pi)$. Positivity permits the [operator monotonicity of the square root](../../../hilbert-space.md#operator-monotonicity-of-the-square-root) and hence $K^{1/2}\preceq Q^{1/2}$; the [spectral representations](../../../hilbert-space.md#projection-valued-measure) in the question identify the top spectral values and give the same gap inequality.

## 4

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

[Hamiltonian Monte Carlo](../../../statistical-inference.md#hamiltonian-monte-carlo) augments the position $x$ by an independent momentum $p\sim N(0,M)$ and uses the [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function)

$$
H(x,p)=-\log\pi(x)+\frac12p^TM^{-1}p.
$$

From the current $x$, draw a fresh $p$, apply a fixed number of [leapfrog steps](../../../classical-mechanics.md#leapfrog-integration) to approximate [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow), and obtain $(x',p')$. The [Metropolis–Hastings acceptance probability](../../../statistical-inference.md#metropolis-hastings-acceptance-probability) is

$$
1\wedge\exp\{H(x,p)-H(x',p')\};
$$

otherwise retain $x$. Momentum negation may be included to make the proposal explicitly reversible. The leapfrog map is volume preserving and reversible, while the acceptance step corrects its discretization error, leaving $\pi$ invariant after the momentum is discarded.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a sufficiently regular [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion) with $D=\sigma\sigma^T/2$, a density $\pi$ is stationary if and only if it solves the stationary [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation)

$$
\nabla\mathbin\cdot\left(b\pi-\nabla\mathbin\cdot(D\pi)\right)=0,
$$

with integrable [Fokker-Planck probability current](../../../probability-theory.md#fokker-planck-probability-current) and boundary conditions that make its outward flux vanish. Here $(\nabla\mathbin\cdot(D\pi))_i=\sum_j\partial_j(D_{ij}\pi)$.

For the displayed parametrization, assume

$$
\pi(x)=Z^{-1}e^{-H(x)},
$$

where $Z<\infty$, that $D(x)$ is symmetric positive semidefinite, and that $Q(x)$ is antisymmetric. Substituting $\nabla\pi=-\pi\nabla H$ and the stated $\Gamma$ into the probability current cancels all $D$ terms. The remaining divergence is

$$
-\sum_{i,j}\partial_i\partial_j(Q_{ij}\pi)=0,
$$

because the second derivatives are symmetric in $i,j$ whereas $Q_{ij}=-Q_{ji}$. Thus these conditions, together with the boundary and regularity assumptions, imply stationarity. More generally, the divergence equation above is the exact necessary and sufficient condition; within this construction, $\pi\propto e^{-H}$ and antisymmetric $Q$ are the standard way to satisfy it.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

[Invariant distribution of an Itô diffusion](../../../stochastic-calculus.md#invariant-distribution-of-an-ito-diffusion), specialized to [Underdamped Langevin dynamics](../../../stochastic-calculus.md#underdamped-langevin-dynamics), has density

$$
\pi(x,p)=Z^{-1}\exp\left\{-U(x)-\frac{\lVert p\rVert^2}{2\eta}\right\}.
$$

Thus $X$ has density proportional to $e^{-U(x)}$, and conditionally and marginally $P\sim N(0,\eta I_d)$. The Hamiltonian transport between $x$ and $p$ preserves this density, while the [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process) in momentum has exactly that Gaussian invariant law.

The [Euler-Maruyama method](../../../stochastic-calculus.md#euler-maruyama-method) with step size $\delta$ and independent $\xi_k\sim N(0,I_d)$ is

$$
\begin{aligned}
P_{k+1}
&=P_k-\gamma\delta P_k-\eta\delta\nabla U(X_k)
+\sqrt{2\gamma\eta\delta}\,\xi_k,\\
X_{k+1}&=X_k+\delta P_k.
\end{aligned}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
