# Paper 215

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20215.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20215.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)

## 1

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Center the board at the origin and map each white square $(i,j)$ to

$$
(u,v)=\left(\frac{i+j}{2},\frac{i-j}{2}\right).
$$

The white squares become the integer points of the diamond

$$
D_n=\{(u,v)\in\mathbb Z^2:|u|+|v|\leq n\},
$$

and a bishop move changes exactly one coordinate. From $(u,v)$ the chain can move first to $(u,0)$ and then to $(0,0)$, since both points lie in $D_n$. Reversing such paths connects any two states, so the [bishop random walk](../../../markov-process.md#bishop-random-walk) is an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In the diamond coordinates, the horizontal line through $(u,v)$ has $2(n-|u|)+1$ points and the vertical line has $2(n-|v|)+1$ points. There is a numerical constant $a>0$, independent of $n$ and of the starting point, such that the walk enters the middle diamond $D_{n/2}$ within two steps with probability at least $a$. To see this, suppose $|u|\leq|v|$, so $|u|\leq n/2$. With probability at least $1/2$ the first move uses the longer horizontal line, and a fixed positive fraction of its choices have $|v'|\leq n/4$. From $(u,v')$, the vertical line has length at least $3n/2$, is chosen with probability bounded below, and a fixed positive fraction of its points satisfy $|u'|+|v'|\leq n/2$. The case $|v|\leq|u|$ is symmetric.

Now couple two copies. Independently use the preceding construction until both lie in $D_{n/2}$, an event having probability at least $a^2$ in two steps. From $(u,v)$ and $(u',v')$ in that diamond, their horizontal line ranges overlap in at least $n+1$ values. A [maximal coupling](../../../probability-and-statistics.md#maximal-coupling) of the next moves can therefore, with probability bounded below, send them to $(u,w)$ and $(u',w)$ for the same $|w|\leq n/2$. Their vertical lines are then identical, and another maximal coupling makes the two states equal with probability bounded below. Thus there are constants $k$ and $b>0$, independent of $n$, for which the two copies coalesce during every block of $k$ steps with conditional probability at least $b$.

The coupling time consequently has a geometric tail. By the [coupling inequality for total variation](../../../probability-and-statistics.md#coupling-inequality-for-total-variation), for each fixed $0<\varepsilon<1$,

$$
t_{\mathrm{mix}}(\varepsilon)\leq k\left\lceil\frac{\log(1/\varepsilon)}{-\log(1-b)}\right\rceil=O_\varepsilon(1).
$$

Since a nontrivial chain has mixing time bounded below by a positive constant, the mixing time has constant order.

## 2

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For every $A\subseteq[n]$, define the [Walsh character](../../../combinatorics.md#walsh-character)

$$
\chi_A(x)=(-1)^{\sum_{i\in A}x_i},
\qquad x\in\{0,1\}^n.
$$

These $2^n$ functions form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). For the lazy walk, which stays put with probability $1/2$ and otherwise flips a uniformly chosen coordinate,

$$
P\chi_A=\left(1-\frac{|A|}{n}\right)\chi_A.
$$

Hence the eigenvalue $1-k/n$ has multiplicity $\binom nk$, for $0\leq k\leq n$.

The supplied [spectral upper bound for total variation mixing](../../../markov-process.md#spectral-upper-bound-for-total-variation-mixing) gives

$$
4\lVert P^t(x,\cdot)-\pi\rVert_{\mathrm{TV}}^2
\leq\sum_{k=1}^n\binom nk\left(1-\frac kn\right)^{2t}
\leq\left(1+e^{-2t/n}\right)^n-1
\leq e^{ne^{-2t/n}}-1.
$$

At $t=\tfrac12n\log n+Cn$, the last expression is $e^{e^{-2C}}-1$. Choosing $C=C(\varepsilon)$ so that this is at most $4\varepsilon^2$ proves

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)leq\frac12n\log n+C(\varepsilon)n.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Assume without loss of generality that $\mu(f)-\nu(f)=r\sigma$ and let $m=(\mu(f)+\nu(f))/2$. By [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality),

$$
\mu(f<m)\leq\frac4{r^2},
\qquad
\nu(f\geq m)\leq\frac4{r^2}.
$$

Using the event $\{f\geq m\}$ in the variational definition of [total variation distance](../../../probability-and-statistics.md#total-variation-distance) gives

$$
\lVert\mu-\nu\rVert_{\mathrm{TV}}
\geq1-\frac8{r^2}.
$$

Start the lazy hypercube walk at $0^n$ and write

$$
\Phi(x)=\sum_{i=1}^n(-1)^{x_i}=n-2\sum_{i=1}^nx_i.
$$

This is an eigenfunction with eigenvalue $1-1/n$, so

$$
\mathbb E_0\Phi(X_t)=n(1-1/n)^t,
\qquad \mathbb E_\pi\Phi=0.
$$

The stated variance estimates allow the preceding lemma with $\sigma=\sqrt n$ and

$$
r=\sqrt n(1-1/n)^t.
$$

For $t=\tfrac12n\log n-Cn$, $r^2$ is bounded below by a constant multiple of $e^{2C}$, uniformly for all sufficiently large $n$. Choosing $C=C(\varepsilon)$ so that $1-8/r^2>\varepsilon$, and absorbing finitely many small $n$ into the constant, proves

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)geq\frac12n\log n-C(\varepsilon)n.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The urn count $X_t^{(n)}$ is the [lumped Markov chain](../../../markov-process.md#lumped-markov-chain) obtained from the lazy hypercube walk by recording its [Hamming weight](../../../coding-theory.md#hamming-weight). Starting from $0^n$, the hypercube law is uniform on every Hamming sphere, as is its stationary law conditional on the sphere. Consequently the total variation distance of the full walk from stationarity equals that of its Hamming-weight projection.

Parts (a) and (b) place every fixed-$\varepsilon$ mixing time at

$$
\frac12n\log n+O_\varepsilon(n).
$$

The window $O(n)$ is little-$o(n\log n)$, so the sequence exhibits [cutoff for Markov chains](../../../markov-process.md#cutoff-for-markov-chains) at $\frac12n\log n$ with an order-$n$ window.

## 3

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The [Dirichlet form of a Markov chain](../../../markov-process.md#dirichlet-form-of-a-markov-chain) is

$$
\mathcal E(f,g)=\frac12\sum_{x,y\in S}
\pi(x)P(x,y)(f(x)-f(y))(g(x)-g(y)).
$$

When $P$ is [reversible](../../../markov-process.md#reversible-markov-chain), this equals $\langle f,(I-P)g\rangle_\pi$.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

For a finite reversible lazy chain, the [relaxation time](../../../markov-process.md#relaxation-time) is $t_{\mathrm{rel}}=1/\gamma$, where $\gamma=1-\lambda_2$ is the [spectral gap](../../../linear-operator-theory.md#spectral-gap). Its [spectral profile](../../../markov-process.md#spectral-profile) is

$$
\Lambda(r)=\inf_{\pi_{\min}\leq\pi(A)\leq r}\lambda(A),
\qquad
\lambda(A)=\inf_{f\in c_0^+(A)}
\frac{\mathcal E(f,f)}{\operatorname{Var}_\pi(f)}.
$$

The variational characterization of the spectral gap is

$$
\gamma=\inf_{f\text{ nonconstant}}
\frac{\mathcal E(f,f)}{\operatorname{Var}_\pi(f)}.
$$

Every class $c_0^+(A)$ is contained in the class over which this last infimum is taken, so $\lambda(A)\geq\gamma$ and $\Lambda(r)\geq\gamma$. Therefore

$$
\boxed{t_{\mathrm{rel}}=\frac1\gamma\geq\frac1{\Lambda(r)}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $N=|V_n|$. Since the degrees lie between $1$ and $\Delta$,

$$
\pi_{\min}\geq\frac1{\Delta N}.
$$

The [Generalized Cheeger inequality](../../../markov-process.md#generalized-cheeger-inequality) and $\Phi_*(u)\geq\Phi_*(c)\geq\alpha$ for $u\leq c$ give

$$
\Lambda(u)\geq\frac{\alpha^2}{2}
\qquad(\pi_{\min}\leq u\leq c).
$$

For all larger $u$, part (a) gives $\Lambda(u)\geq1/t_{\mathrm{rel}}$. Split the supplied spectral-profile integral at $c$ to obtain

$$
\begin{aligned}
t_{\mathrm{mix}}(\varepsilon)
&\leq2\int_{4\pi_{\min}}^{4/\varepsilon}\frac{du}{u\Lambda(u)}\\
&\lesssim_{\alpha,c,\Delta}
\log\frac1{\pi_{\min}}+t_{\mathrm{rel}}\log\frac1\varepsilon\\
&\lesssim\log N+t_{\mathrm{rel}}\log(1/\varepsilon).
\end{aligned}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Under the standard intended reading that the added edges form a [perfect matching](../../../graph-theory.md#perfect-matching) between $G_n$ and $H_n$, the claim follows as follows. Degrees in $M_n$ remain bounded in terms of $\Delta$. For $A\subseteq V(M_n)$, write $A_G=A\cap V(G_n)$ and $A_H=A\cap V(H_n)$. The matching contributes at least $\bigl||A_G|-|A_H|\bigr|$ boundary edges, while expansion inside $G_n$ contributes a constant multiple of $\min\{|A_G|,n-|A_G|\}$. A case split according as $|A_G|\leq n/2$ or $|A_G|>n/2$ shows

$$
|\partial_{M_n}A|\geq c_{\alpha,\Delta}
\min\{|A|,2n-|A|\}.
$$

Thus $M_n$ has a uniform [Cheeger constant](../../../markov-process.md#cheeger-constant). [Cheeger inequality](../../../markov-process.md#cheeger-inequality) gives a uniformly bounded relaxation time, while $\pi_{\min}\asymp1/n$. The usual spectral mixing estimate, or part (b), then gives $t_{\mathrm{mix}}\lesssim\log n$.

If “adding $n$ edges” permits all $G_n$ vertices to attach to the same vertex of $H_n$, the assertion is false as written. Take $H_n$ to be a path and attach every vertex of the expander to one endpoint. A walk started at the other endpoint needs order $n^2$ time to reach the attachment endpoint, so its mixing time is not $O(\log n)$. The perfect-matching interpretation is therefore necessary.

## 4

↑ **Parent:** [Paper 215](paper-215.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For a path $\gamma=(v_0,e_1,v_1,\ldots,e_k,v_k)$, its $\ell$-length is $\sum_{j=1}^k\ell(e_j)$. The corresponding [path metric](../../../graph-theory.md#path-metric) is

$$
\rho(x,y)=\inf_{\gamma:x\to y}\sum_{e\in\gamma}\ell(e).
$$

Because every edge length is at least one, $\rho(x,y)\geq1$ whenever $x\ne y$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Let $D=\max_{x,y}\rho(x,y)$ and let $\pi$ be the invariant distribution. Iterating the assumed [Wasserstein contraction](../../../probability-and-statistics.md#wasserstein-contraction) gives

$$
\rho_K(P^t(x,\cdot),\pi)
=\rho_K(P^t(x,\cdot),\pi P^t)
\leq e^{-\alpha t}\rho_K(\delta_x,\pi)
\leq e^{-\alpha t}D.
$$

Since $\rho(x,y)\geq\mathbf1_{\{x\ne y\}}$, the [coupling characterization of total variation distance](../../../probability-and-statistics.md#coupling-characterization-of-total-variation-distance) implies

$$
\lVert P^t(x,\cdot)-\pi\rVert_{\mathrm{TV}}
\leq\rho_K(P^t(x,\cdot),\pi)
\leq e^{-\alpha t}D.
$$

The right side is at most $\varepsilon$ when

$$
t\geq\frac1\alpha(\log D-\log\varepsilon),
$$

which proves the claimed mixing bound.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For any two states $X,Y$, the closed neighbourhood of $X\cup Y$ has at most $2s(\Delta+1)\leq2n/3$ vertices. The remaining induced graph therefore has at least $n/3$ vertices and maximum degree at most $\Delta$, so the [greedy independent-set bound](../../../graph-theory.md#greedy-independent-set-bound) supplies an independent set $Z$ of size $s$ there. No vertex of $Z$ is adjacent to a vertex of $X\cup Y$. Replace the elements of $X$ one at a time by the elements of $Z$, and then replace the elements of $Z$ one at a time by those of $Y$. Every intermediate set is independent, and every prescribed swap has positive transition probability. Hence the chain is irreducible.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

If distinct states $X,Y$ communicate in one step, they differ by a unique removed vertex and a unique inserted vertex. Consequently

$$
P(X,Y)=\frac1{sn}=P(Y,X).
$$

**Thus the transition matrix is symmetric, so [detailed balance](../../../markov-process.md#detailed-balance) holds for the uniform distribution on $S$. Irreducibility makes this invariant distribution unique.**

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Give the state graph the unit-edge [path metric](../../../graph-theory.md#path-metric). The construction in part (i) shows that its diameter is at most $2s$. It remains to couple one step from neighbouring states $X=A\cup\{x\}$ and $Y=A\cup\{y\}$.

Pair the choice $x$ in the first chain with $y$ in the second, and pair every $a\in A$ with itself; use the same proposed vertex $v$ in both chains. When the pair $(x,y)$ is removed, the chains coalesce whenever $v$ is not in the closed neighbourhood of $A$. This has probability at least

$$
C=\frac{n-(s-1)(\Delta+1)}{sn}.
$$

When a common $a\in A$ is removed, the distance can increase from one to at most two only if $v$ lies in one of the closed neighbourhoods of $x$ and $y$, an event of probability at most

$$
B=\frac{2(\Delta+1)}n.
$$

Therefore

$$
\mathbb E[\rho(X_1,Y_1)]
\leq1-C+B
\leq1-\frac1{sn},
$$

where the last inequality uses $n\geq3s(\Delta+1)$. The [Path coupling theorem](../../../markov-process.md#path-coupling-theorem) extends this contraction to arbitrary starting distributions. Since $1-1/(sn)\leq e^{-1/(sn)}$, part (a) with diameter at most $2s$ yields

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)
\leq sn\log\frac{2s}{\varepsilon}
\lesssim sn\log(s/\varepsilon).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
