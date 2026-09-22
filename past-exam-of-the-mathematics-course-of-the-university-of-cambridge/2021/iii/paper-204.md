# Paper 204

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_204.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_204.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $\alpha=\inf_{r\geq1}a_r/r$. The inequality $a_n/n\geq\alpha$ gives $\liminf_na_n/n\geq\alpha$. Fix $r$ and write $n=qr+s$, where $0\leq s<r$. Repeated subadditivity gives $a_n\leq qa_r+a_s$ when $s>0$, with the evident omission when $s=0$. Since the finitely many remainders $a_s$ are bounded,

$$
\limsup_{n\to\infty}\frac{a_n}{n}\leq\frac{a_r}{r}.
$$

Taking the infimum over $r$ proves the [Fekete lemma](../../../real-analysis.md#fekete-s-lemma):

$$
\boxed{\lim_{n\to\infty}\frac{a_n}{n}=\inf_{r\geq1}\frac{a_r}{r}}.
$$

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Splitting any $(m+n)$-step [self-avoiding walk](../../../combinatorics.md#self-avoiding-walk) after $m$ steps and translating its remaining segment to the origin injects it into an ordered pair of an $m$-step and an $n$-step self-avoiding walk. Hence $b_{m+n}\leq b_mb_n$. The sequence $a_n=\log b_n$ is subadditive, so the [Fekete lemma](../../../real-analysis.md#fekete-s-lemma) gives

$$
\lim_{n\to\infty}\frac{\log b_n}{n}=\inf_{n\geq1}\frac{\log b_n}{n}.
$$

Exponentiating proves existence of the [connective constant](../../../combinatorics.md#connective-constant) $\kappa=\lim_nb_n^{1/n}$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

After the first of the four possible steps, a self-avoiding walk has at most three choices at every stage because it cannot immediately reverse its preceding step. Thus $b_n\leq4\cdot3^{n-1}$ and $\kappa\leq3$. On the other hand, every sequence of $n$ north or east steps is self-avoiding, so $b_n\geq2^n$ and $\kappa\geq2$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Consider walks assembled from blocks $E$, $EN^k$, and $ES^k$ with $k\geq1$. Their horizontal coordinate increases once in every block, and within each vertical line they move monotonically, so every such walk is self-avoiding. If $c_n$ counts these walks by total length, its [ordinary generating function](../../../commutative-algebra.md#ordinary-generating-function) is

$$
\sum_{n\geq0}c_nz^n
=\frac1{1-\left(z+2\sum_{k\geq1}z^{k+1}\right)}
=\frac{1-z}{1-2z-z^2}.
$$

Its positive dominant singularity is $z=\sqrt2-1$, so $\lim_nc_n^{1/n}=1+\sqrt2$. Since $b_n\geq c_n$,

$$
\boxed{\kappa\geq1+\sqrt2>2}.
$$

## 2

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In [site percolation](../../../site-percolation.md) on the three-dimensional cubic lattice, each vertex $v\in\mathbb Z^3$ is independently open with probability $p$ and closed with probability $1-p$. Thus $\mathbb P_p$ is the Bernoulli product measure on $\{0,1\}^{\mathbb Z^3}$, and open paths are nearest-neighbour paths all of whose vertices are open.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [percolation probability](../../../probability-theory.md#percolation-probability) and [percolation critical probability](../../../probability-theory.md#percolation-critical-probability) are

$$
\boxed{\theta(p)=\mathbb P_p(0\leftrightarrow\infty),
\qquad
p_c=\inf\{p:\theta(p)>0\}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The events $A_n$ decrease, and an open path from $0$ reaches every $\partial\Lambda_n$ exactly when the open cluster of $0$ is infinite. Therefore [continuity from above of a measure](../../../measure-theory.md#continuity-from-above-of-a-measure) gives

$$
\mathbb P_p(A_n)\downarrow\mathbb P_p(0\leftrightarrow\infty)=\theta(p).
$$

Each $A_n$ depends on finitely many sites, so $p\mapsto\mathbb P_p(A_n)$ is a polynomial and hence [continuous](../../../calculus.md#continuous-function). Given $\varepsilon>0$, choose $n$ with $\mathbb P_p(A_n)<\theta(p)+\varepsilon$. For $p'\downarrow p$, monotonicity and the finite-event continuity yield

$$
\theta(p)\leq\theta(p')\leq\mathbb P_{p'}(A_n)\longrightarrow\mathbb P_p(A_n)<\theta(p)+\varepsilon.
$$

**Thus $\theta(p')\to\theta(p)$ from the right.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For every $v\in\mathbb Z^3$, sample independent $U_v\sim\operatorname{Unif}[0,1]$ and set $\eta_p(v)=\mathbf1_{\{U_v\leq p\}}$. Then each $\eta_p$ has the required Bernoulli product law and $\eta_p\leq\eta_{p'}$ whenever $p\leq p'$. This is the [monotone coupling of Bernoulli percolation](../../../probability-theory.md#monotone-coupling-of-bernoulli-percolation).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Within the monotone coupling, $I_p$ increases with $p$ and

$$
\bigcup_{p'<p}I_{p'}=\{M<p\}.
$$

Taking a countable cofinal sequence $p'\uparrow p$ and using [continuity from below of a measure](../../../measure-theory.md#continuity-from-below-of-a-measure) gives

$$
\lim_{p'\uparrow p}\theta(p')=\mathbb P(M<p).
$$

Since $\{M<p\}\subseteq I_p$, subtraction from $\theta(p)=\mathbb P(I_p)$ proves

$$
\boxed{\theta(p)-\lim_{p'\uparrow p}\theta(p')=\mathbb P(I_p\cap\{M=p\})}.
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Use the standard theorem that supercritical Bernoulli percolation on $\mathbb Z^3$ has a unique infinite open cluster almost surely. Fix $p>p_c$ and choose $q\in(p_c,p)$. Almost surely $\eta_q$ has an infinite cluster somewhere. On $I_p$, the origin and that cluster lie in the unique infinite $\eta_p$-cluster, so a finite $\eta_p$-open path joins them. Almost surely every label on this finite path is strictly below $p$; increasing $q$ to some $r<p$ above those finitely many labels makes the origin percolate in $\eta_r$. Hence $I_p\subseteq\{M<p\}$ up to a null event, and part e gives left continuity at $p$. Together with part c, $\theta$ is continuous on $(p_c,1]$.

## 3

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $\omega\in\{0,1\}^{E}$, write $o(\omega)=|\eta(\omega)|$ and $c(\omega)=|E|-o(\omega)$. The [random-cluster model](../../../site-percolation.md#random-cluster-model) is

$$
\phi_{p,q}(\omega)=\frac1{Z_{p,q}}p^{o(\omega)}(1-p)^{c(\omega)}q^{k(\omega)}.
$$

For $0\leq p\leq1$ and $q\geq1$, its [positive association of the random-cluster model](../../../site-percolation.md#positive-association-of-the-random-cluster-model) states that increasing functions $f,g$ satisfy $\phi_{p,q}(fg)\geq\phi_{p,q}(f)\phi_{p,q}(g)$.

For the two parallel edges $e_1,e_2$, the four unnormalized weights for $00,10,01,11$ are respectively

$$
(1-p)^2q^2,quad p(1-p)q,quad p(1-p)q,quad p^2q.
$$

For the increasing events $A=\{e_1\text{ open}\}$ and $B=\{e_2\text{ open}\}$, positive association is equivalent to $w_{00}w_{11}\geq w_{10}w_{01}$, which reduces to $q\geq1$. It therefore fails whenever $p,q\in(0,1)$.

At $p=1/2$, all factors involving the number of open edges are equal, so the weight is proportional to $q^{k(\omega)}$. The smallest possible component count is one. Dividing numerator and denominator by $q$ and sending $q\downarrow0$ leaves equal weight precisely on connected spanning subgraphs, proving the stated [uniform connected-subgraph limit of the random-cluster model](../../../site-percolation.md#uniform-connected-subgraph-limit-of-the-random-cluster-model).

Finally let $p,q\downarrow0$ with $q/p\to0$, and let $N=|V|$. Fix a spanning tree $\tau$. The ratio of the weight of $\omega$ to that of $\tau$ is

$$
\left(\frac{p}{1-p}\right)^{o(\omega)-N+1}q^{k(\omega)-1}
=(1-p)^{N-1-o(\omega)}p^{d(\omega)}\left(\frac qp\right)^{k(\omega)-1},
$$

where $d(\omega)=o(\omega)+k(\omega)-N\geq0$. Equality $d=0$ means that the open graph is a forest. The ratio tends to zero unless $d=0$ and $k=1$, which means precisely that $\omega$ is a spanning tree. All spanning trees have equal weight, so the limiting law is the [uniform spanning-tree limit of the random-cluster model](../../../site-percolation.md#uniform-spanning-tree-limit-of-the-random-cluster-model):

$$
\phi_{p,q}(\omega)\longrightarrow
\begin{cases}
1/|\mathcal T|,&\omega\in\mathcal T,\\
0,&\omega\notin\mathcal T,
\end{cases}
$$

where $\mathcal T$ is the set of spanning trees of $G$.

## 4

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [contact process](../../../stochastic-process.md#contact-process) on $\mathbb Z$ has states $\xi_t(x)\in\{0,1\}$. Each infected site recovers at rate $\mu$, and infection passes across each oriented nearest-neighbour edge at rate $\lambda$. For the [graphical representation of the contact process](../../../stochastic-process.md#graphical-representation-of-the-contact-process), put independent rate-$\mu$ recovery marks on each vertical time line and independent rate-$\lambda$ infection arrows on each oriented nearest-neighbour edge. Then $y\in\xi_t^A$ exactly when a forward path from some $(x,0)$ with $x\in A$ reaches $(y,t)$ by moving upward, following arrows, and avoiding recovery marks.

If $A\subseteq B$, every path starting in $A$ also starts in $B$, so $\xi_t^A\subseteq\xi_t^B$. A path starts in $A\cup B$ exactly when it starts in one of the two sets, which proves [additivity of the contact process](../../../stochastic-process.md#additivity-of-the-contact-process):

$$
\xi_t^{A\cup B}=\xi_t^A\cup\xi_t^B.
$$

The event $\xi_t^A\cap B\ne\varnothing$ says that a graphical path runs from $A\times\{0\}$ to $B\times\{t\}$. Reflecting the time interval about $t/2$ and reversing every arrow preserves the joint law of the independent Poisson processes, and the path now runs from $B$ to $A$. This proves [duality of the contact process](../../../stochastic-process.md#duality-of-the-contact-process):

$$
\mathbb P_{\lambda,\mu}(\xi_t^A\cap B\ne\varnothing)
=\mathbb P_{\lambda,\mu}(\xi_t^B\cap A\ne\varnothing).
$$

The [survival probability of the contact process](../../../stochastic-process.md#survival-probability-of-the-contact-process) is

$$
\theta(\lambda,\mu)=\mathbb P_{\lambda,\mu}(\xi_t^{\{0\}}\ne\varnothing\text{ for every }t\geq0),
$$

and $\lambda_c(\mu)=\inf\{\lambda:\theta(\lambda,\mu)>0\}$. By duality and translation invariance,

$$
\mathbb P_{\lambda,\mu}(\xi_t^{\mathbb Z}(x)=1)
=\mathbb P_{\lambda,\mu}(\xi_t^{\{x\}}\ne\varnothing)
=\mathbb P_{\lambda,\mu}(\xi_t^{\{0\}}\ne\varnothing).
$$

The events on the right decrease with $t$ because the empty state is absorbing, and their intersection is eternal survival. Therefore

$$
\boxed{\theta(\lambda,\mu)=\lim_{t\to\infty}\mathbb P_{\lambda,\mu}(\xi_t^{\mathbb Z}(x)=1)}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
