# Paper 214

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_214.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_214.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
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
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put

$$
\alpha=\inf_{k\geq1}\frac{x_k}{k}.
$$

Fix $k\geq1$ and write $n=qk+r$ with $0\leq r<k$. Repeated [subadditivity](../../../real-analysis.md#subadditive-sequence) gives

$$
x_n\leq qx_k+x_r,
$$

so

$$
\frac{x_n}{n}\leq\frac{qk}{n}\frac{x_k}{k}+\frac{x_r}{n}.
$$

The finitely many values $x_0,\ldots,x_{k-1}$ are bounded, hence

$$
\limsup_{n\to\infty}\frac{x_n}{n}\leq\frac{x_k}{k}.
$$

Taking the infimum over $k$ gives $\limsup x_n/n\leq\alpha$, while the definition of $\alpha$ gives $x_n/n\geq\alpha$ for every $n$. Therefore

$$
\boxed{\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\geq1}\frac{x_k}{k}.}
$$

This is [Fekete lemma](../../../real-analysis.md#fekete-s-lemma).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Let

$$
a_n=-\log\mathbb P_p(0\leftrightarrow e_n).
$$

The events $\{0\leftrightarrow e_n\}$ and $\{e_n\leftrightarrow e_{n+m}\}$ are increasing events of [bond percolation](../../../bond-percolation.md). The [FKG inequality](../../../probability-inequality.md#fkg-inequality) and translation invariance give

$$
\mathbb P_p(0\leftrightarrow e_{n+m})
\geq \mathbb P_p(0\leftrightarrow e_n)
\mathbb P_p(e_n\leftrightarrow e_{n+m})
=\mathbb P_p(0\leftrightarrow e_n)
\mathbb P_p(0\leftrightarrow e_m).
$$

Thus $(a_n)$ is a [subadditive sequence](../../../real-analysis.md#subadditive-sequence). Since every probability is positive for $p>0$, [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) applies and gives

$$
\boxed{\phi(p)=\lim_{n\to\infty}a_n/n
=\inf_{n\geq1}\left[-\frac1n\log\mathbb P_p(0\leftrightarrow e_n)\right].}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

By the [union bound](../../../probability-inequality.md#boole-s-inequality),

$$
\mathbb P_p(0\leftrightarrow\partial B(n))
\leq\sum_{z\in\partial B(n)}
\mathbb P_p(0\leftrightarrow z).
$$

Hence some $z\in\partial B(n)$ has connection probability at least the left side divided by $|\partial B(n)|$. Some coordinate of $z$ equals $n$ or $-n$. A coordinate permutation and reflection of $\mathbb Z^d$ sends that face to the face $x_1=n$ and preserves the [bond percolation](../../../bond-percolation.md) law. Its image $x$ therefore satisfies

$$
\boxed{\mathbb P_p(0\leftrightarrow x)
\geq\frac{\mathbb P_p(0\leftrightarrow\partial B(n))}{|\partial B(n)|}.}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Write

$$
q_n=\mathbb P_p(0\leftrightarrow\partial B(n)),
\qquad a_n=\mathbb P_p(0\leftrightarrow e_n).
$$

Since $e_n\in\partial B(n)$, $q_n\geq a_n$, and therefore

$$
\limsup_{n\to\infty}-\frac1n\log q_n\leq\phi(p).
$$

For the opposite inequality, choose $x=(n,x_2,\ldots,x_d)$ as in part (ii). Reflection about $x$ sends $0$ to $2ne_1$ and preserves the lattice. Thus the increasing events $\{0\leftrightarrow x\}$ and $\{x\leftrightarrow2ne_1\}$ have the same probability. The [FKG inequality](../../../probability-inequality.md#fkg-inequality) yields

$$
a_{2n}\geq\mathbb P_p(0\leftrightarrow x)^2
\geq\left(\frac{q_n}{|\partial B(n)|}\right)^2.
$$

Consequently

$$
-\frac1n\log q_n
\geq-\frac1{2n}\log a_{2n}
-\frac1n\log|\partial B(n)|.
$$

The polynomial boundary-size estimate makes the last term tend to zero, while the first tends to $\phi(p)$. Hence

$$
\boxed{\lim_{n\to\infty}-\frac1n\log q_n=\phi(p).}
$$

## 2

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Because $p<p_c=\widetilde p_c$, choose a finite set $S\ni0$ with $\phi_p(S)=\rho<1$. Let $L$ exceed the $\ell^\infty$-distance from $0$ to every endpoint of an edge in $\partial S$, and put

$$
q_n=\mathbb P_p(0\leftrightarrow\partial B(n)).
$$

On the one-arm event to distance $n>L$, take the first oriented boundary edge $(x,y)\in\partial S$ used by an open self-avoiding path. The connection $0\xleftarrow{S}x$, the open edge $(x,y)$, and the remaining connection from $y$ to $\partial B(n)$ occur disjointly. The [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) and translation invariance therefore give

$$
\begin{aligned}
q_n
&\leq p\sum_{(x,y)\in\partial S}
\mathbb P_p(0\xleftarrow{S}x)
\mathbb P_p(y\leftrightarrow\partial B(n))\\
&\leq\phi_p(S)q_{n-L}=\rho q_{n-L}.
\end{aligned}
$$

Iteration yields $q_n\leq\rho^{\lfloor n/L\rfloor}$ up to an inessential finite-scale adjustment. Since $p<1$, each of the finitely many remaining $q_n$ is strictly below one, so reducing the exponent if necessary produces a constant $c>0$ valid for every $n\geq1$:

$$
\boxed{\mathbb P_p(0\leftrightarrow\partial B(n))\leq e^{-cn}.}
$$

This is the finite-size proof of [exponential decay of subcritical percolation](../../../probability-theory.md#exponential-decay-of-subcritical-percolation).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

By [Tonelli theorem](../../../measure-theory.md#tonelli-theorem),

$$
\chi(p)=\mathbb E_p|\mathcal C|
=\sum_{x\in\mathbb Z^d}\mathbb P_p(0\leftrightarrow x).
$$

If $p<p_c$, part (a) bounds the summand by $e^{-c\lVert x\rVert_\infty}$. There are only polynomially many vertices at each radius, so the series converges and $\chi(p)<\infty$.

Conversely, suppose $\chi(p)<\infty$. Then $p<1$. Choose $q>p$ so close to $p$ that

$$
2d\,\frac{q-p}{1-p}\,\chi(p)<1.
$$

Use the standard [sprinkling coupling for Bernoulli percolation](../../../probability-theory.md#sprinkling-coupling-for-bernoulli-percolation): first expose the $p$-open clusters, then independently open each remaining edge with probability $\alpha=(q-p)/(1-p)$. Explore the $q$-cluster of the origin cluster by following sprinkled edges. Each discovered $p$-cluster has at most $2d$ times its number of vertices as many incident edges, so the exploration is dominated by a [Galton-Watson process](../../../probability-and-statistics.md#galton-watson-process) of mean at most $2d\alpha\chi(p)<1$. This process dies out almost surely, and hence there is no infinite $q$-open cluster. Thus $q\leq p_c$, and $p<q$ implies $p<p_c$. Therefore

$$
\boxed{\chi(p)<\infty\iff p<p_c.}
$$

## 3

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [voltage](../../../markov-process.md#voltage) with boundary values $u(a)$ and $u(b)$ is a function $u:V\to\mathbb R$ that is harmonic at every other vertex:

$$
\sum_yc(x,y)(u(x)-u(y))=0,
\qquad x\notin\{a,b\}.
$$

A [current flow](../../../markov-process.md#current-flow) is an antisymmetric function $i(x,y)=-i(y,x)$ satisfying Kirchhoff's node law $\sum_yi(x,y)=0$ away from its source and sink. Voltage and current are related by [Ohm's law](../../../electromagnetism.md#ohm-s-law),

$$
i(x,y)=c(x,y)(u(x)-u(y)).
$$

The [effective resistance](../../../markov-process.md#effective-resistance) is the voltage drop divided by the total current from $a$ to $b$. Equivalently, it is the voltage drop generated by a unit current flow:

$$
R_{\mathrm{eff}}(a,b)=\frac{u(a)-u(b)}{\sum_yi(a,y)}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $A=\{a,b\}$ and let $\tau_x^+=\min\{t\geq1:X_t=x\}$. The conductance-hitting identity for an [electrical network](../../../markov-process.md#electrical-network) is

$$
\mathbb P_x(\tau_D<\tau_x^+)
=\frac{1}{c(x)R_{\mathrm{eff}}(x,D)},
\qquad c(x)=\sum_yc(x,y),
$$

where the vertices of $D$ are wired together. It follows by taking the hitting probability of $D$ before returning to $x$ as a voltage and computing its total current out of $x$.

Split the walk into successive excursions from $x$. The first excursion that hits $A$ determines whether $a$ or $b$ is hit first. Its conditional probability of hitting $a$ is at most the probability that an arbitrary excursion hits $a$, divided by the probability that it hits $A$. Hence

$$
\begin{aligned}
\mathbb P_x(\tau_a<\tau_b)
&\leq
\frac{\mathbb P_x(\tau_a<\tau_x^+)}
{\mathbb P_x(\tau_A<\tau_x^+)}\\
&=\boxed{\frac{R_{\mathrm{eff}}(x,A)}{R_{\mathrm{eff}}(x,a)}}.
\end{aligned}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $v$ be the voltage with $v(a)=1$, $v(b)=0$, and harmonic values at every other vertex. For any other admissible $f$, write $f=v+g$, where $g(a)=g(b)=0$. Its [discrete Dirichlet energy](../../../markov-process.md#discrete-dirichlet-energy) expands as

$$
\mathcal E(f)=\mathcal E(v)+\mathcal E(g)
+\sum_{x,y}c(x,y)(v(x)-v(y))(g(x)-g(y)).
$$

Discrete summation by parts turns the cross term into

$$
2\sum_xg(x)\sum_yc(x,y)(v(x)-v(y))=0,
$$

because $v$ is harmonic in the interior and $g$ vanishes at the boundary. Thus $v$ minimizes the energy. Under a unit voltage drop, its energy equals the total current from $a$ to $b$, namely the [effective conductance](../../../markov-process.md#effective-conductance) $1/R_{\mathrm{eff}}(a,b)$. Therefore the [Dirichlet principle](../../../calculus-of-variations.md#dirichlet-principle) gives

$$
\boxed{
\frac1{R_{\mathrm{eff}}(a,b)}
=\inf_{f(a)=1,\,f(b)=0}
\frac12\sum_{x,y}(f(x)-f(y))^2c(x,y).}
$$

## 4

↑ **Parent:** [Paper 214](paper-214.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [spanning tree](../../../combinatorics.md#spanning-tree) of a finite connected graph $G$ is a connected acyclic subgraph containing every vertex. A [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) is a random spanning tree chosen uniformly from the finite set of all spanning trees of $G$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For an infinite locally finite recurrent connected graph, take an increasing exhaustion by finite connected subgraphs and sample a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) in each. The restrictions to any fixed finite edge set converge in distribution; on a recurrent graph the free and wired limits coincide and form one tree. This infinite-volume law is called the uniform spanning tree of the recurrent graph.

It can be generated by [Wilson's algorithm](../../../combinatorics.md#wilson-s-algorithm). Fix a root and an enumeration of the remaining vertices. Starting with the root, run a random walk from the first vertex not yet in the tree until it hits the existing tree, erase its loops chronologically, and add the resulting path. Recurrence ensures every walk hits the finite tree almost surely. Repeating this operation produces the infinite uniform spanning tree, independently of the enumeration.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Exhaust $\mathbb Z^2$ by finite boxes $G_n$ and let $T_n$ be a [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) of $G_n$. Every finite tree satisfies the [handshaking lemma](../../../combinatorics.md#degree-sum-formula), so

$$
\frac1{|V(G_n)|}\sum_{v\in V(G_n)}\deg_{T_n}(v)
=\frac{2(|V(G_n)|-1)}{|V(G_n)|}\longrightarrow2.
$$

Choose the root uniformly from $V(G_n)$. The proportion of roots within any fixed distance of the boundary tends to zero, and the rooted trees converge locally to the uniform spanning tree $T$ of $\mathbb Z^2$. Since every degree is at most four, expectations also converge. Translation invariance therefore gives

$$
\mathbb E[\deg_T(0)]=2.
$$

The four edges incident to $0$ have equal inclusion probability by the rotations and reflections of the square lattice. If that common probability is $r$, then $4r=\mathbb E\deg_T(0)=2$. Consequently

$$
\boxed{\mathbb P(e\in T)=\frac12}
$$

for every edge $e$ by translation invariance.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
