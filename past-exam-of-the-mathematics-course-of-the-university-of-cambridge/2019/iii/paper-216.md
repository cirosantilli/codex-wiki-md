# Paper 216

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_216.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_216.pdf)

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
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Writing $s_i=2x_i-1$, the edge term rewards neighboring computers having the same infection state, as in a ferromagnetic [Ising model](../../../statistical-physics.md#ising-model), while $-\frac1{10}\sum_i x_i$ expresses a mild prior preference for the rarer uninfected state. Thus the prior encodes local transmission over the network without assuming independent infections.

The observation likelihood is

$$
L(x)=\prod_{i\in V_2}\frac14\mathbf1_{\{x_i=1\}}
\prod_{i\in V_1\setminus V_2}\left(\frac34\right)^{x_i}.
$$

Consequently the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is

$$
p(x_V\mid V_2)
\propto
\exp\left[
\sum_{\{i,j\}\in E}(2x_i-1)(2x_j-1)
-\frac1{10}\sum_i x_i
\right]L(x).
$$

This remains a binary pairwise [Markov random field](../../../statistical-model.md#markov-random-field) on a tree. To find its [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate), run [max-product belief propagation](../../../statistical-model.md#max-product-belief-propagation): send a two-entry message in each direction along every edge, then backtrack from the maximizing root state. Each message examines four state pairs, and the maximum degree is bounded, so the total cost is

$$
\boxed{O(|V|).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The posterior mean of the number infected is

$$
\mathbb E\left[\sum_{i\in V}X_i\,middle|\,V_2\right]
=\sum_{i\in V}\mathbb P(X_i=1\mid V_2).
$$

Run [sum-product belief propagation](../../../statistical-model.md#sum-product-belief-propagation) on the tree to compute every exact one-vertex posterior marginal. Summing their probabilities of state one gives the requested mean. Messages have fixed size and every directed edge is processed once, so the exact computation costs

$$
\boxed{O(|V|).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

After the sum-product messages have been computed, draw exact independent posterior configurations by sampling a root from its marginal and then sampling each child from its conditional distribution given its parent. For sample $m$, set

$$
I_m=\mathbf1\left\{\sum_{i\in V}X_i^{(m)}>2|V_2|\right\},
\qquad
\widehat q=\frac1N\sum_{m=1}^NI_m.
$$

Then $\widehat q$ is unbiased and

$$
\operatorname{Var}(\widehat q)=\frac{q(1-q)}N.
$$

Taking $N=1000$ attains the required bound. Message computation costs $O(|V|)$ and each exact sample costs $O(|V|)$, so with the prescribed fixed number of samples the overall cost is

$$
\boxed{O(|V|).}
$$

## 2

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Given the current state $x=(x_1,\ldots,x_d)$, a [Random-scan Gibbs sampler](../../../statistical-inference.md#random-scan-gibbs-sampler) chooses $I$ uniformly from $\{1,\ldots,d\}$, leaves $x_{-I}$ unchanged, and samples the new coordinate from the complete conditional distribution

$$
X_I'\sim\pi(dx_I\mid x_{-I}).
$$

Its transition kernel is

$$
K(x,dy)=\frac1d\sum_{i=1}^d
\pi(dy_i\mid x_{-i})\,\delta_{x_{-i}}(dy_{-i}),
$$

and it leaves $\pi$ invariant.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Because $f$ is a continuous bijection $\mathbb R\to\mathbb R$, it is a Borel isomorphism. Conditional on $X_{-i}=x_{-i}$, the $i$th coordinate of $F(X)$ has the pushforward of $\pi(dx_i\mid x_{-i})$ under $f$. Therefore applying one $K$-update and then $F$ has exactly the same law as applying one $Q$-update to $F(x)$, using the same random coordinate.

Formally, for every Borel set $A$,

$$
Q(F(x),A)=K(x,F^{-1}(A)).
$$

Composition preserves this conjugacy, so induction on $t$ gives

$$
Q^t(F(x),A)=K^t(x,F^{-1}(A)).
$$

Hence

$$
\boxed{Y\sim K^t(x,\cdot)\implies F(Y)\sim Q^t(F(x),\cdot).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Total variation is invariant under a measurable bijection with measurable inverse. Using part (b),

$$
\begin{aligned}
\|Q^t(F(x),\cdot)-\nu\|_{\mathrm{TV}}
&=\sup_A|K^t(x,F^{-1}(A))-\pi(F^{-1}(A))|\\
&=\|K^t(x,\cdot)-\pi\|_{\mathrm{TV}}
\leq2^{-t}.
\end{aligned}
$$

Every $z\in\mathbb R^d$ equals $F(x)$ for a unique $x$, so

$$
\boxed{\|Q^t(z,\cdot)-\nu\|_{\mathrm{TV}}\leq2^{-t}
\quad\text{for every }z.}
$$

## 3

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put

$$
S(x)=\sum_{i=1}^dp(x,i).
$$

The normalizing identity

$$
\int S(x)\nu(dx)
=\sum_i\int\nu(dx_{-i})\int\mu(dx_i\mid x_{-i})=d
$$

shows that

$$
\boxed{\pi(dx)=\frac{S(x)}d\nu(dx)}
$$

is a probability measure. If $x$ and $y$ differ only in coordinate $i$, the transition density from $x$ to $y$ is $p(x,i)\mu(y_i\mid x_{-i})/S(x)$. Therefore

$$
\begin{aligned}
\pi(x)K(x,y)
&=\frac1d\nu(x)p(x,i)\mu(y_i\mid x_{-i})\\
&=\frac1d\nu(x_{-i})
\mu(x_i\mid x_{-i})\mu(y_i\mid x_{-i}),
\end{aligned}
$$

which is symmetric in $x_i,y_i$. Thus detailed balance holds and the [Tempered Gibbs sampler](../../../statistical-inference.md#tempered-gibbs-sampler) is $\pi$-reversible.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The summand intended in the question is $d,h(X(t))/S(X(t))$. Under stationarity,

$$
\mathbb E_\pi\left[\frac{d,h(X)}{S(X)}\right]
=\int\frac{d,h(x)}{S(x)}\frac{S(x)}d\nu(dx)
=\int h\,d\nu=H.
$$

Moreover $S(x)\geq dc_1$, so the summand is bounded by $1/c_1$. A stationary geometrically ergodic Markov chain satisfies the [Markov-chain law of large numbers](../../../statistical-inference.md#markov-chain-law-of-large-numbers); hence

$$
\widehat H_n=\frac1n\sum_{t=1}^n
\frac{d,h(X(t))}{S(X(t))}
\longrightarrow H
$$

almost surely, and therefore in probability. In particular,

$$
\boxed{\Pr(|\widehat H_n-H|>\epsilon)\to0.}
$$

## 4

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\theta=(\beta,\pi)$ and regard $X_U$ as the [latent variable](../../../statistical-modelling.md#latent-variable). At iteration $t$, the E-step forms

$$
Q(\theta\mid\theta^{(t)})
=\mathbb E_{\theta^{(t)}}[
\log p(Y,X_U,X_O,\theta)
\mid Y,X_O].
$$

The M-step updates

$$
\theta^{(t+1)}\in\arg\max_\theta
Q(\theta\mid\theta^{(t)}).
$$

This is the [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) for the posterior objective: including $\log p(\theta)$ in the complete-data log density makes the maximizer a [maximum a posteriori estimate](../../../statistical-inference.md#maximum-a-posteriori-estimate) rather than a maximum-likelihood estimate.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $U_i=\{j:(i,j)\notin O\}$ and let $x_{i,O}$ denote the observed entries in row $i$. Conditional on the parameters, different rows of the missing design are independent, while the missing entries within one row are coupled by its Gaussian response. For $z\in\{0,1\}^{U_i}$,

$$
\Pr(X_{i,U_i}=z\mid Y,X_O,\beta,\pi)
\propto
\exp\left[-\frac{(Y_i-x_i(z)^T\beta)^2}{2\sigma^2}\right]
\prod_{j\in U_i}\pi_j^{z_j}(1-\pi_j)^{1-z_j}.
$$

Normalizing this expression over the $2^{|U_i|}$ configurations and multiplying over rows gives the full conditional distribution of $X_U$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Ignoring constants, the complete-data log posterior is

$$
-\frac1{2\sigma^2}\|Y-X\beta\|^2
-\frac1{2\sigma_\beta^2}\|\beta\|^2
+\sum_{i,j}\{X_{ij}\log\pi_j+(1-X_{ij})\log(1-\pi_j)\}.
$$

Take conditional expectations under $(\beta^{(t)},\pi^{(t)})$. Define

$$
A=\frac1{2\sigma^2}\mathbb E[X^TX\mid Y,X_O,\theta^{(t)}]
+\frac1{2\sigma_\beta^2}I,
$$



$$
d=A^{-1}\frac{\mathbb E[X\mid Y,X_O,\theta^{(t)}]^TY}{2\sigma^2},
\quad
r_j=\sum_i\mathbb E[X_{ij}\mid\cdots],
\quad q_j=n-r_j.
$$

Completing the square gives

$$
Q=-(\beta-d)^TA(\beta-d)
+\sum_j\{r_j\log\pi_j+q_j\log(1-\pi_j)\}
+\text{constant}.
$$

For $v\ne0$,

$$
v^TAv=\frac1{2\sigma^2}\mathbb E\|Xv\|^2
+\frac1{2\sigma_\beta^2}\|v\|^2>0,
$$

so $A$ is positive definite. Exact rowwise expectations require summing over $2^{|U_i|}$ states. Thus the cost is exponential in the largest number of missing covariates in one row, more precisely $\sum_i2^{|U_i|}$ times a polynomial factor for accumulating first and second moments.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Positive definiteness makes the quadratic term uniquely maximal at

$$
\boxed{\beta^{(t+1)}=d.}
$$

For each $j$, maximize the concave function $r_j\log\pi_j+q_j\log(1-\pi_j)$. Its interior critical point is

$$
\boxed{\pi_j^{(t+1)}=\frac{r_j}{r_j+q_j}=\frac{r_j}{n}.}
$$

The same formula gives the appropriate boundary value when $r_j=0$ or $q_j=0$.

## 5

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Introduce $Z_{ij}\in\{0,1\}$, where $Z_{ij}=1$ means that the observation came from the structural-zero component. Conditional on the parameters,

$$
\Pr(Z_{ij}=1\mid Y_{ij})=
\begin{cases}
\displaystyle\frac{\pi_j}{\pi_j+(1-\pi_j)e^{-\alpha_i\beta_j}},&Y_{ij}=0,\\
0,&Y_{ij}>0.
\end{cases}
$$

Given $Z$, the nonstructural observations are independent Poisson variables. Using shape-rate parameterization and the stated unit-rate priors, the remaining Gibbs updates are

$$
\alpha_i\mid-\sim\operatorname{Gamma}\left(
1+\sum_j(1-Z_{ij})Y_{ij},
1+\sum_j(1-Z_{ij})\beta_j
\right),
$$



$$
\beta_j\mid-\sim\operatorname{Gamma}\left(
1+\sum_i(1-Z_{ij})Y_{ij},
1+\sum_i(1-Z_{ij})\alpha_i
\right),
$$



$$
\pi_j\mid-\sim\operatorname{Beta}\left(
1+\sum_iZ_{ij},
1+n-\sum_iZ_{ij}
\right).
$$

Alternating these four standard-distribution updates defines the requested [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) for the [Zero-inflated Poisson distribution](../../../discrete-probability-distribution.md#zero-inflated-poisson-distribution) posterior.

## 6

↑ **Parent:** [Paper 216](paper-216.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let

$$
H(x,p)=U(x)+\frac12p^Tp
$$

be the [Hamiltonian](../../../classical-mechanics.md#hamiltonian). The [Hamiltonian Monte Carlo](../../../statistical-inference.md#hamiltonian-monte-carlo) proposal is accepted with the [Metropolis–Hastings acceptance probability](../../../statistical-inference.md#metropolis-hastings-acceptance-probability)

$$
\boxed{
\alpha=1\wedge
\exp\{H(X_t,P_t)-H(x(L\varepsilon),p(L\varepsilon))\}.}
$$

The leapfrog map is volume preserving and reversible after momentum reversal, so no proposal-density Jacobian appears.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For $U(x)=x^Tx/2$, one leapfrog step is

$$
\begin{pmatrix}x'\\p'\end{pmatrix}
=M_\varepsilon
\begin{pmatrix}x\\p\end{pmatrix},
\qquad
M_\varepsilon=
\begin{pmatrix}
(1-\varepsilon^2/2)I&\varepsilon I\\
(-\varepsilon+\varepsilon^3/4)I&(1-\varepsilon^2/2)I
\end{pmatrix}.
$$

Therefore $L$ steps give

$$
\boxed{
\begin{pmatrix}x(L\varepsilon)\\p(L\varepsilon)\end{pmatrix}
=M_\varepsilon^L
\begin{pmatrix}x(0)\\p(0)\end{pmatrix},}
$$

which is a linear transformation.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For fixed $L$, expansion of the matrix in part (b) gives

$$
(M_\varepsilon^L)^TM_\varepsilon^L
=
\begin{pmatrix}
(1+O(\varepsilon^4))I&O(\varepsilon^3)I\\
O(\varepsilon^3)I&(1+O(\varepsilon^4))I
\end{pmatrix}.
$$

Hence its largest eigenvalue is $1+O(\varepsilon^3)$. With $z=(x(0),p(0))$ and $z'=M_\varepsilon^Lz$,

$$
H(z')=\frac12\|z'\|^2
\leq(1+C_0\varepsilon^3)H(z).
$$

For each fixed starting state, or uniformly on any bounded set of starting states, this implies

$$
H(z')-H(z)\leq C_1\varepsilon^3.
$$

Using $e^{-u}\geq1-u$ for $u\geq0$ in the acceptance formula gives

$$
\boxed{1-C\varepsilon^3\leq\alpha\leq1}
$$

for sufficiently small $\varepsilon$. The constant necessarily depends on a bound for $\|z\|$: a uniform pointwise constant over all of $\mathbb R^{2d}$ would be impossible because the energy error is quadratic in the starting state.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
