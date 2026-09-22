# Paper 215

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_215.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_215.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Start the [random-to-top card shuffle](../../../markov-process.md#random-to-top-card-shuffle) from a fixed ordering and let $T$ be the first time every card has been selected. Once a card has been selected, its location relative to the other selected cards is determined by their most recent selection times. At $T$ these times have a uniformly random strict order, so the deck is uniform and independent of the event $\{T=t\}$. Thus $T$ is a [strong stationary time](../../../markov-process.md#strong-stationary-time), and

$$
d_{\mathrm{TV}}(t)\leq\mathbb P(T>t).
$$

The [coupon collector problem](../../../discrete-probability-distribution.md#coupon-collector-problem) gives $T=n\log n+O_{\mathbb P}(n)$, so for $c\to\infty$,

$$
d_{\mathrm{TV}}(n\log n+cn)\longrightarrow0.
$$

Before all cards have been selected, the unselected cards form the bottom block of the deck in their original relative order. At time $n\log n-cn$, with $c\to\infty$ sufficiently slowly, the number $U$ of unselected cards tends to infinity in probability. Choose $k\to\infty$ with $\mathbb P(U\geq k)\to1$. The bottom $k$ cards are then in their original relative order, whereas under the uniform distribution this has probability $1/k!$. Hence

$$
d_{\mathrm{TV}}(n\log n-cn)\longrightarrow1.
$$

The random-to-top shuffle therefore has [cutoff for Markov chains](../../../markov-process.md#cutoff-for-markov-chains) at $n\log n$ with window $O(n)$.

The [top-to-random card shuffle](../../../markov-process.md#top-to-random-card-shuffle) is the time reversal of the [random-to-top card shuffle](../../../markov-process.md#random-to-top-card-shuffle) under the uniform stationary distribution. Equivalently, their step distributions on the symmetric group are carried into one another by permutation inversion, which preserves total variation from uniform. Their mixing profiles agree, so **top-to-random has the same cutoff at $n\log n$ with window $O(n)$**.

## 2

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The chain is a random walk on the finite abelian group $(\mathbb Z/n\mathbb Z)^d$, so its stationary distribution is uniform and its characters diagonalize the transition operator. For one coordinate and $\theta=2\pi k/n$, the eigenvalue is

$$
\lambda_{p}(\theta)=\frac12+
rac p2e^{i\theta}+
rac{1-p}{2}e^{-i\theta}.
$$

Uniformly in $p\in[0,1]$,

$$
|\lambda_p(\theta)|^2
\leq1-c\min\left\{\frac{k^2}{n^2},1\right\}
$$

for an absolute $c>0$. Hence the one-coordinate chi-squared distance after $t\geq n^2$ is at most $Ce^{-ct/n^2}$. The coordinates evolve independently, so the product formula for chi-squared distance gives

$$
1+\chi^2_d(t)
=\prod_{j=1}^d(1+\chi^2_j(t))
\leq\exp\left(Cd e^{-ct/n^2}\right).
$$

The [chi-squared divergence](../../../probability-and-statistics.md#chi-squared-divergence) bound on [total variation distance](../../../probability-and-statistics.md#total-variation-distance) now yields

$$
\boxed{t_{\mathrm{mix}}=O(n^2\log(d+1)),}
$$

uniformly in $p_1,\ldots,p_d$.

For $d=1$, the first nonconstant character has eigenvalue modulus $1-O(n^{-2})$, uniformly in $p$. Testing against its real or imaginary part gives a fixed positive total-variation distance until time $cn^2$. Thus

$$
\boxed{t_{\mathrm{mix}}=\Theta(n^2)\quad(d=1).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the monotone grand coupling in every coordinate: at each step use the same attempted move for chains started from the bottom and top states, censoring moves that leave the interval. The two copies coalesce after the lower copy has accumulated enough upward drift and boundary censoring has removed their initial separation. Away from the boundary, one step has mean displacement

$$
\frac13-\frac16=\frac16.
$$

Standard exponential concentration for sums of bounded independent increments shows that for every fixed $C>6$ the one-coordinate coupling time $\tau$ satisfies

$$
\mathbb P(\tau>Cn)\leq e^{-c_Cn}.
$$

All other initial states lie between the extremal copies. Coupling the $d$ coordinates independently and using the [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P(\text{some coordinate has not coupled by }Cn)
\leq d e^{-c_Cn}=o(1),
$$

because $\log d=o(n)$. The [coupling inequality for total variation](../../../probability-and-statistics.md#coupling-inequality-for-total-variation) therefore gives

$$
\boxed{t_{\mathrm{mix}}=O(n).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Take $d=1$ and start from the lower endpoint. The stationary distribution of this birth-death chain satisfies detailed balance with

$$
\frac{\pi(k+1)}{\pi(k)}=\frac{1/3}{1/6}=2,
$$

so it is concentrated within $O(1)$ of the upper endpoint $n$. Before reaching that region the walk has drift $1/6$. The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) and exponential concentration therefore imply that its hitting time of $n-O(1)$ is

$$
6n+O_{\mathbb P}(\sqrt n).
$$

At time $(6-\varepsilon)n$ the chain is still macroscopically below the stationary region with probability tending to one, so its total-variation distance tends to one. Under the monotone coupling from part (b), by time $(6+\varepsilon)n$ the extremal copies have coalesced with probability tending to one, so the distance tends to zero. Therefore the family has

$$
\boxed{\text{cutoff at }6n\text{ with an }O(\sqrt n)\text{ window}.}
$$

## 3

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Couple two [noisy voter model](../../../markov-process.md#noisy-voter-model) chains by choosing the same update vertex, the same refresh coin and refreshed spin, and, for a voter update, the same chosen neighbor. Let $D_t$ be their [Hamming distance](../../../coding-theory.md#hamming-distance). If $G$ is $r$-regular, conditioning on the current disagreement set gives

$$
\begin{aligned}
\mathbb E[D_{t+1}\mid D_t]
&=D_t-\frac{D_t}{n}
+\frac{1-p}{n}\sum_{v\in V}
\frac{|N(v)\cap D_t|}{r}\\
&=\left(1-\frac pn\right)D_t,
\end{aligned}
$$

because every disagreeing vertex is counted in exactly $r$ neighbor sets. Therefore

$$
\mathbb E D_t\leq n\left(1-\frac pn\right)^t.
$$

The [coupling inequality for total variation](../../../probability-and-statistics.md#coupling-inequality-for-total-variation) and $\mathbf1_{\{\sigma_t\ne\sigma_t'\}}\leq D_t$ give

$$
\boxed{\max_{\sigma,\sigma'}
\|P^t(\sigma,\cdot)-P^t(\sigma',\cdot)\|_{\mathrm{TV}}
\leq n\left(1-\frac pn\right)^t.}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For a nonregular graph, use the degree-weighted Hamming metric

$$
W_t=\sum_{v\in V}\deg(v)
\mathbf1_{\{\sigma_t(v)\ne\sigma_t'(v)\}}.
$$

Under the same coupling,

$$
\begin{aligned}
\mathbb E[W_{t+1}-W_t\mid\sigma_t,\sigma_t']
={}&-\frac1n\sum_{v\in D_t}\deg(v)\\
&+\frac{1-p}{n}\sum_v\deg(v)
\frac{|N(v)\cap D_t|}{\deg(v)}\\
={}&-\frac pnW_t.
\end{aligned}
$$

Here the final double sum equals $\sum_{u\in D_t}\deg(u)=W_t$. Since $W_0\leq\sum_v\deg(v)=2|E|$ and $W_t\geq1$ whenever the chains differ,

$$
\boxed{\max_{\sigma,\sigma'}
\|P^t(\sigma,\cdot)-P^t(\sigma',\cdot)\|_{\mathrm{TV}}
\leq2|E|\left(1-\frac pn\right)^t.}
$$

## 4

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $P$ be a finite reversible Markov chain with stationary distribution $\pi$, and write $Q(e)=\pi(u)P(u,v)$ for an oriented transition edge $e=(u,v)$. For every ordered pair $(x,y)$ choose a directed path $\gamma_{xy}$ from $x$ to $y$ using positive-capacity edges, and define the congestion

$$
\rho=\max_e\frac1{Q(e)}
\sum_{x,y:e\in\gamma_{xy}}
\pi(x)\pi(y)|\gamma_{xy}|.
$$

Then the [Canonical paths comparison theorem](../../../markov-process.md#canonical-paths-comparison-theorem) gives the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality)

$$
\boxed{\operatorname{Var}_\pi(f)\leq\rho\,\mathcal E(f,f)}
$$

for every real function $f$, and hence the spectral gap is at least $1/\rho$.

Indeed,

$$
\operatorname{Var}_\pi(f)
=\frac12\sum_{x,y}\pi(x)\pi(y)(f(x)-f(y))^2.
$$

Write each difference as the sum of edge differences along $\gamma_{xy}$ and apply [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
(f(x)-f(y))^2
\leq|\gamma_{xy}|\sum_{e\in\gamma_{xy}}(\nabla_ef)^2.
$$

Interchanging the pair and edge sums, then applying the definition of $\rho$, bounds the result by

$$
\frac\rho2\sum_eQ(e)(\nabla_ef)^2
=\rho\mathcal E(f,f).
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let

$$
m=\max_x\mathbb E_xT_A
$$

and choose $x$ attaining the maximum. For every $t$, the [Strong Markov property](../../../markov-process.md#strong-markov-property) at time $t$ gives

$$
m=\mathbb E_xT_A
\leq t+m\mathbb P_x(T_A>t).
$$

Thus

$$
\mathbb P_x(T_A\leq t)\leq\frac tm.
$$

If $t\geq t_{\mathrm{mix}}(1/4)$, then

$$
\mathbb P_x(X_t\in A)
\geq\pi(A)-\frac14\geq\frac14.
$$

Since $\{X_t\in A\}\subseteq\{T_A\leq t\}$, this is impossible when $t<m/4$. Allowing for integer times, one may take any smaller absolute constant, for example

$$
\boxed{t_{\mathrm{mix}}(1/4)\geq\frac18
\max_x\mathbb E_xT_A.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
