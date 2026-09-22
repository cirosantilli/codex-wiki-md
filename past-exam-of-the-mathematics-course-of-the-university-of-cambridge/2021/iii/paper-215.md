# Paper 215

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_215.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_215.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The laziness of $P=(Q+I)/2$ makes all its eigenvalues nonnegative. Write

$$
1=\lambda_1>\lambda_2\geq\cdots\geq\lambda_{|S|}\geq0.
$$

The [relaxation time](../../../markov-process.md#relaxation-time) is

$$
t_{\mathrm{rel}}=\frac1{1-\lambda_2}.
$$

If $(f_i)$ is an orthonormal eigenbasis of $L^2(\pi)$ with $f_1=1$, the spectral decomposition is

$$
\boxed{\frac{P^t(x,y)}{\pi(y)}
=\sum_{i=1}^{|S|}\lambda_i^tf_i(x)f_i(y).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

On the diagonal,

$$
P^k(x,x)-\pi(x)
=\pi(x)\sum_{i\geq2}\lambda_i^kf_i(x)^2,
$$

so every summand is nonnegative. Let $m=\lceil t_{\mathrm{rel}}\rceil$. For every $i\geq2$,

$$
\lambda_i^{m+1}
\leq\lambda_2^{t_{\mathrm{rel}}}
=\left(1-\frac1{t_{\mathrm{rel}}}\right)^{t_{\mathrm{rel}}}
\leq e^{-1}.
$$

Hence

$$
\frac1{1-\lambda_i}
\leq\frac e{e-1}\frac{1-\lambda_i^{m+1}}{1-\lambda_i}
=\frac e{e-1}\sum_{k=0}^m\lambda_i^k.
$$

Multiply by $\pi(x)f_i(x)^2$ and sum over $i\geq2$ to obtain the required inequality.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The squared $L^2(\pi)$ distance has the diagonal identity

$$
\left\lVert\frac{P^t(x,\mathord\cdot)}{\pi(\mathord\cdot)}-1\right\rVert_{2,\pi}^2
=\frac{P^{2t}(x,x)-\pi(x)}{\pi(x)}.
$$

The diagonal excess is nonnegative and decreases with time. Therefore

$$
(2t+1)\{P^{2t}(x,x)-\pi(x)\}
\leq\sum_{k=0}^\infty\{P^k(x,x)-\pi(x)\}.
$$

Using the identity supplied in the question gives

$$
\left\lVert\frac{P^t(x,\mathord\cdot)}{\pi(\mathord\cdot)}-1\right\rVert_{2,\pi}^2
\leq\frac{\mathbb E_\pi\tau_x}{2t+1}.
$$

At $t=8\mathbb E_\pi\tau_x$ the right side is at most $1/16$, up to the immaterial integer rounding. Thus

$$
\boxed{t_{\mathrm{mix}}^{(2)}(x,1/4)\leq8\mathbb E_\pi\tau_x}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put $T=t_{\mathrm{mix}}^{(2)}(a,1/4)$ and $m=\lceil t_{\mathrm{rel}}\rceil$. The expected local time is

$$
\mathbb E_a\sum_{k=0}^{T-1}\mathbf1_{\{X_k=a\}}
=T\pi(a)+\sum_{k=0}^{T-1}\{P^k(a,a)-\pi(a)\}.
$$

Part c and the supplied return identity give

$$
T\pi(a)\leq8\pi(a)\mathbb E_\pi\tau_a
=8\sum_{k=0}^\infty\{P^k(a,a)-\pi(a)\}.
$$

The second term is bounded by the same infinite sum. Part b now yields

$$
\mathbb E_a\sum_{k=0}^{T-1}\mathbf1_{\{X_k=a\}}
\leq\frac{9e}{e-1}
\sum_{k=0}^m\{P^k(a,a)-\pi(a)\}
\leq\frac{9e}{e-1}\mathbb E_a\sum_{k=0}^m\mathbf1_{\{X_k=a\}}.
$$

**Thus the hinted universal constant $C=9e/(e-1)$ works.**

## 2

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A family exhibits [pre-cutoff for Markov chains](../../../markov-process.md#pre-cutoff-for-markov-chains) if there are constants $0<A<B<\infty$ and times $t_n$ such that its worst-case total-variation distance tends to one at $At_n$ and to zero at $Bt_n$. For irreducible reversible chains, a standard necessary condition for pre-cutoff is the product condition

$$
t_{\mathrm{rel}}^{(n)}=o(t_{\mathrm{mix}}^{(n)}).
$$

The hypothesis that $t_{\mathrm{mix}}^{(n)}/t_{\mathrm{rel}}^{(n)}$ is bounded contradicts this condition, while $t_{\mathrm{mix}}^{(n)}\to\infty$ excludes a bounded-time degeneracy. Hence the family cannot exhibit pre-cutoff.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $\Pi_n(x,y)=\pi_n(y)$. Since $P_n\Pi_n=\Pi_nP_n=\Pi_n$ and $\Pi_n^2=\Pi_n$, the [stationary-reset perturbation of a Markov chain](../../../markov-process.md#stationary-reset-perturbation-of-a-markov-chain) satisfies

$$
\widetilde P_n^t
=\Pi_n+(1-a_n)^t(P_n^t-\Pi_n).
$$

Every row difference from stationarity is multiplied by the nonnegative scalar $(1-a_n)^t$, so

$$
\boxed{
\lVert\widetilde P_n^t(x,\mathord\cdot)-\pi_n\rVert_{\mathrm{TV}}
=(1-a_n)^t
\lVert P_n^t(x,\mathord\cdot)-\pi_n\rVert_{\mathrm{TV}}}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Write $r_n=t_{\mathrm{mix}}^{(n)}/t_{\mathrm{rel}}^{(n)}\to\infty$. Then

$$
a_nt_{\mathrm{mix}}^{(n)}=\sqrt{r_n}\to\infty,
\qquad
a_n^{-1}=\sqrt{t_{\mathrm{rel}}^{(n)}t_{\mathrm{mix}}^{(n)}}=o(t_{\mathrm{mix}}^{(n)}).
$$

By cutoff, at every fixed multiple $c/a_n$ the original chain is still asymptotically unmixed, while part i gives

$$
\widetilde d_n(c/a_n)\longrightarrow e^{-c}.
$$

Thus the new chain crosses between fixed distance levels gradually on the full scale $a_n^{-1}$: for example its $\varepsilon$-mixing times are asymptotic to $a_n^{-1}\log(1/\varepsilon)$. No two fixed multiples of one scale can make the limiting distance respectively one and zero, so the family has no pre-cutoff.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Every nonconstant eigenvalue $\lambda$ of $P_n$ becomes $(1-a_n)\lambda$. Hence, writing $\gamma_n=1/t_{\mathrm{rel}}^{(n)}$,

$$
\widetilde\gamma_n
=1-(1-a_n)(1-\gamma_n)
=a_n+(1-a_n)\gamma_n.
$$

Since

$$
a_nt_{\mathrm{rel}}^{(n)}
=\sqrt{\frac{t_{\mathrm{rel}}^{(n)}}{t_{\mathrm{mix}}^{(n)}}}\to0,
$$

we have $\widetilde t_{\mathrm{rel}}^{(n)}\sim t_{\mathrm{rel}}^{(n)}$. Part ii gives $\widetilde t_{\mathrm{mix}}^{(n)}\asymp a_n^{-1}$, and therefore

$$
\boxed{\frac{\widetilde t_{\mathrm{rel}}^{(n)}}{\widetilde t_{\mathrm{mix}}^{(n)}}
\asymp a_nt_{\mathrm{rel}}^{(n)}
=\sqrt{\frac{t_{\mathrm{rel}}^{(n)}}{t_{\mathrm{mix}}^{(n)}}}
\longrightarrow0.}
$$

## 3

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a path $\Gamma$,

$$
\{f(x)-f(y)\}^2
\leq|\Gamma|\sum_{e\in\Gamma}\{\nabla_ef\}^2
$$

by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Average over $\nu_{xy}$, multiply by $\widetilde Q(x,y)$, and sum. Reversing the order of summation in the definition of the two [Dirichlet forms](../../../markov-process.md#dirichlet-form-of-a-markov-chain) gives

$$
\mathcal E_{\widetilde P}(f,f)\leq B\mathcal E_P(f,f).
$$

Let $M=\max_x\pi(x)/\widetilde\pi(x)$. The variational formula for variance gives

$$
\operatorname{Var}_\pi f
=\min_c\sum_x\pi(x)(f(x)-c)^2
\leq M\operatorname{Var}_{\widetilde\pi}f.
$$

Take a nonconstant eigenfunction attaining the Rayleigh quotient $\gamma$ for $P$. Then

$$
\widetilde\gamma
\leq\frac{\mathcal E_{\widetilde P}(f,f)}
{\operatorname{Var}_{\widetilde\pi}f}
\leq MB\frac{\mathcal E_P(f,f)}{\operatorname{Var}_\pi f}
=\boxed{MB\gamma}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Choose the uniform distribution on shortest paths equivariantly under graph automorphisms. Automorphisms preserve distances and send uniform shortest paths to uniform shortest paths, so vertex transitivity makes

$$
\widetilde f(x)=\sum_{y\sim x}f(x,y)
$$

constant in $x$. Summing this constant over vertices counts each path-edge incidence at most twice:

$$
n\widetilde f(x)
=\sum_x\widetilde f(x)
\leq2\sum_{u,v\in V}\mathbb E_{\nu_{uv}}|\Gamma_{uv}|
\leq2n^2\Delta.
$$

Thus $\widetilde f(x)\leq2n\Delta$, and each nonnegative summand satisfies

$$
\boxed{f(e)\leq2n\Delta}.
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Compare simple random walk $P$ with the independent sampler $\widetilde P(x,y)=\pi(y)=1/n$, whose spectral gap is one. Both stationary distributions are uniform. Route each transition $(x,y)$ of the sampler along a uniformly selected shortest path. For a directed graph edge $e$,

$$
Q(e)=\frac1{nd},
\qquad
\widetilde Q(x,y)=\frac1{n^2},
\qquad
|\Gamma_{xy}|\leq\Delta.
$$

Part i therefore bounds the congestion by

$$
B\leq nd\frac{\Delta}{n^2}f(e)
\leq2d\Delta^2.
$$

Part a, equivalently the [Canonical paths comparison theorem](../../../markov-process.md#canonical-paths-comparison-theorem), gives

$$
1=\widetilde\gamma\leq B\gamma,
\qquad
\boxed{\frac1\gamma\leq2d\Delta^2}.
$$

## 4

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For each fixed output state $y$, the right-shift part has exactly two predecessors, each contributing $1/3$, and the left-shift part also has exactly two predecessors, each contributing $1/6$. Thus every column sum is

$$
2\left(\frac13\right)+2\left(\frac16\right)=1.
$$

The transition matrix is doubly stochastic, so the uniform law

$$
\pi(y)=2^{-n}
$$

is invariant.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Track on the lifted integer line the coordinate refreshed at each step. It is a random walk $R_t$ with right-step probability $2/3$ and left-step probability $1/3$. Every visited residue modulo $n$ has had its bit replaced by an independent fair bit. Consequently the first time all residues have been visited is a [strong stationary time](../../../markov-process.md#strong-stationary-time) for this [shift-refresh chain on a hypercube](../../../markov-process.md#shift-refresh-chain-on-a-hypercube).

For the upper bound, reaching level $n$ visits every residue, so the refresh time is at most $\tau_n$. The supplied moments give

$$
\mathbb E\tau_n=3n,\qquad
\operatorname{Var}(\tau_n)=24n.
$$

For any sequence $w_n$ with $w_n/\sqrt n\to\infty$, [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) and the strong-stationary-time bound imply

$$
d_{\mathrm{TV}}(3n+w_n)
\leq\mathbb P(\tau_n>3n+w_n)\longrightarrow0.
$$

For the lower bound, choose integers $b_n$ such that

$$
\sqrt n\ll b_n\ll w_n,\qquad b_n=o(n),
$$

and consider $\tau_{n-2b_n}\wedge\tau_{-b_n}$. Its supplied mean is $3n-6b_n+o(1)$ and its variance is $O(n)$; after replacing $w_n$ by a sequence with $\sqrt n\ll w_n\ll n$, take for example $b_n=\lfloor\sqrt{w_n\sqrt n}\rfloor$. This satisfies the displayed scale separation, and the supplied moment bounds show

$$
\mathbb P\{\tau_{n-2b_n}\wedge\tau_{-b_n}\leq3n-w_n\}\longrightarrow0.
$$

Before that exit, the visited interval has length less than $n-b_n$, so at least $b_n$ coordinates retain their initial values.

Start the chain from the all-zero vector. Conditional on the explored path, the number of one-bits is binomial with at most $n-b_n$ trials, whereas under stationarity it is $\operatorname{Bin}(n,1/2)$. Since $b_n/\sqrt n\to\infty$, standard binomial concentration separates these two laws; for instance the event

$$
\left\{\text{number of ones}\leq\frac n2-\frac{b_n}{4}\right\}
$$

has probability tending to one for the chain and to zero under $\pi$. Therefore

$$
d_{\mathrm{TV}}(3n-w_n)\longrightarrow1.
$$

The transition from one to zero occurs in an $o(n)$ window around $3n$, proving total-variation cutoff with cutoff time $3n$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
