# Paper 204

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_204.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_204.pdf)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A cylinder event in $\{0,1\}^{E(G)}$ is an event determined by the states of finitely many edges. It is increasing when $\omega\in A$ and $\omega'\geq\omega$ coordinatewise imply $\omega'\in A$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $\mu_n$ be the [uniform spanning tree](../../../combinatorics.md#uniform-spanning-tree) measure on the finite connected induced graph $G_n$. Uniform spanning-tree edge indicators are negatively associated: increasing events depending on disjoint edge sets have nonpositive covariance. Together with the spatial Markov property, this implies the free-boundary monotonicity under graph enlargement: for every increasing cylinder event $A$, $\mu_n(A)$ is eventually nonincreasing once $G_n$ contains all edges on which $A$ depends.

Define the [free uniform spanning forest](../../../combinatorics.md#free-uniform-spanning-forest) measure by

$$
\mu_F(A)=\lim_{n\to\infty}\mu_n(A)
$$

for increasing cylinder events. These limits determine a unique probability measure, independent of the exhaustion; equivalently, $\mu_n$ converges weakly to $\mu_F$ on the product space.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix a finite nonempty vertex set $K$. Once $G_n$ contains $K$ and every edge incident to it, every spanning tree of $G_n$ contains an edge of the finite cut

$$
\partial_EK=\{uv:u\in K,\ v\notin K\},
$$

because otherwise $K$ is disconnected from the rest of $G_n$. Hence

$$
\mu_n(\text{every edge of }\partial_EK\text{ is absent})=0,
$$

and the same holds in the weak limit. If the free spanning forest had a finite component, its vertex set would be some finite connected $K$ and all edges of $\partial_EK$ would be absent. Taking the countable union over finite $K$ proves that every component is infinite almost surely.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Because $T$ itself is a tree, every finite induced connected exhaustion has the unique spanning tree consisting of all its edges. Thus its free spanning forest is deterministically $T$.

By the stated transience criterion, choose an edge $e=uv$ whose two complementary subtrees are transient. Run [Wilson algorithm rooted at infinity](../../../combinatorics.md#wilson-algorithm-rooted-at-infinity) first from $u$. With positive probability its loop-erased walk remains forever in the $u$-side. Starting next from $v$, there is likewise positive conditional probability that its walk remains forever in the $v$-side. On this event the two rays never use $e$, so $e$ is absent from the [wired uniform spanning forest](../../../combinatorics.md#wired-uniform-spanning-forest). The wired law is therefore not the deterministic free law.

## 2

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Fix $\epsilon>0$ and choose a cylinder event $B$ with $\mathbb P_p(A\mathbin\triangle B)<\epsilon$. Translate $B$ far enough that $B$ and $\phi(B)$ depend on disjoint edge sets. They are independent, while automorphism invariance gives $\phi(A)=A$. The symmetric-difference inclusion supplied in the question gives

$$
\left|\mathbb P_p(A)-\mathbb P_p(B\cap\phi(B))\right|\leq2\epsilon.
$$

Also $|\mathbb P_p(A)-\mathbb P_p(B)|<\epsilon$, and independence gives $\mathbb P_p(B\cap\phi(B))=\mathbb P_p(B)^2$. Letting $\epsilon\downarrow0$ yields

$$
\mathbb P_p(A)=\mathbb P_p(A)^2,
$$

so $\mathbb P_p(A)\in\{0,1\}$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The number $N_\infty$ is invariant under lattice automorphisms, so part a makes it almost surely equal to one constant in $\{0,1,2,\ldots,\infty\}$. For $p>p_c$ the constant is nonzero.

Suppose it were a finite $k\geq2$. As boxes increase to $\mathbb Z^d$, with positive probability one box meets all $k$ infinite clusters. On that event, open a finite collection of edges inside the box joining those clusters. The [finite-energy property of Bernoulli percolation](../../../probability-theory.md#finite-energy-property-of-bernoulli-percolation) gives the modified event positive probability, but it has fewer than $k$ infinite clusters. This contradicts almost-sure constancy. Hence the only possibilities are

$$
\boxed{N_\infty=1\quad\text{almost surely}
\qquad\text{or}\qquad
N_\infty=\infty\quad\text{almost surely}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The open descendants of any vertex form a [Galton-Watson process](../../../probability-and-statistics.md#galton-watson-process) with offspring distribution $\operatorname{Bin}(k,p)$. If $kp\leq1$, it dies out almost surely, so $N_\infty=0$.

If $kp>1$, let $\theta>0$ be its survival probability. At level $n$, each vertex begins an independent descendant subtree; the event that its edge to its parent is closed while its descendant open cluster is infinite has probability $(1-p)\theta>0$. Thus the number of such vertices at level $n$ is binomial with $k^n$ trials and a fixed positive success probability. For every fixed $M$, the probability of at least $M$ successes tends to one. Their infinite clusters are separated by their closed parent edges, so $\mathbb P(N_\infty\geq M)=1$ for every $M$, and hence $N_\infty=\infty$ almost surely.

## 3

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) says that for increasing cylinder events $A$ and $B$ under product bond percolation,

$$
\mathbb P_p(A\mathbin\square B)
\leq\mathbb P_p(A)\mathbb P_p(B),
$$

where $A\mathbin\square B$ is the event that $A$ and $B$ have disjoint finite witness edge sets.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $A_n$ be the increasing cylinder event that an open path joins $0$ to the boundary of the box $[-n,n]^d$. If two edge-disjoint open paths run from $0$ to infinity, then $A_n\mathbin\square A_n$ occurs for every $n$. Therefore the [Van den Berg-Kesten inequality](../../../bond-percolation.md#van-den-berg-kesten-inequality) gives

$$
\mathbb P_p(\text{two edge-disjoint open paths }0\leftrightarrow\infty)
\leq\lim_{n\to\infty}\mathbb P_p(A_n)^2
=\theta(p)^2,
$$

where continuity from above identifies $\lim_n\mathbb P_p(A_n)=\theta(p)$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $\omega\in\{0,1\}^{E(G)}$, write $o(\omega)$ and $c(\omega)$ for its numbers of open and closed edges and $k(\omega)$ for the number of connected components of the open spanning subgraph. The free [random-cluster model](../../../site-percolation.md#random-cluster-model) is

$$
\boxed{\mathbb P_{\mathrm{FK}}^{p,q}(\omega)
=\frac1{Z_G(p,q)}
p^{o(\omega)}(1-p)^{c(\omega)}q^{k(\omega)}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Put $s=1-p$. On the four-cycle, the total unnormalized weight is

$$
Z=p^4q+4p^3sq+6p^2s^2q^2+4ps^3q^3+s^4q^4.
$$

The event $N\leftrightarrow S$ contains all configurations with zero or one closed edge and exactly two of the six configurations with two closed edges, so its weight is

$$
p^4q+4p^3sq+2p^2s^2q^2.
$$

Divide numerator and denominator by $q$. As $s\to0$ and $sq\to\infty$, the omitted numerator terms are $o(1+2s^2q)$, while the middle denominator terms are

$$
o(1+s^4q^3).
$$

Consequently

$$
\boxed{\mathbb P_{\mathrm{FK}}^{p,q}(N\leftrightarrow S)
=(1+o(1))
\frac{2(1-p)^2q+1}{(1-p)^4q^3+1}.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Take $A=\{N\leftrightarrow S\}$ and let $s=1-p\downarrow0$ with

$$
q=s^{-3/2}.
$$

Then $sq\to\infty$, $s^2q\to0$, and $s^4q^3=s^{-1/2}\to\infty$. Part d gives $\mathbb P_{\mathrm{FK}}^{p,q}(A)\to0$.

On a four-cycle, $A\mathbin\square A$ occurs exactly when all four edges are open, because the two length-two paths from $N$ to $S$ are the only disjoint witnesses. Hence

$$
\mathbb P_{\mathrm{FK}}^{p,q}(A\mathbin\square A\mid A)
=\frac{p^4q}
{p^4q+4p^3sq+2p^2s^2q^2}
\longrightarrow1.
$$

Choosing $s$ sufficiently small gives the two numerical inequalities in the question.

## 4

↑ **Parent:** [Paper 204](paper-204.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Project $X$ to its label in $\mathbb Z^2$. At each step the label makes a nearest-neighbor move with probability $4/5$ and holds with probability $1/5$ when $X$ crosses between layers. This lazy planar random walk is recurrent because ordinary random walk on $\mathbb Z^2$ is recurrent.

Whenever the label returns to that of $x_0$, the layer coordinate belongs to a two-state irreducible chain, and there is a uniformly positive chance to equal the original layer. Infinitely many label returns therefore give infinitely many returns to $x_0$. Thus simple random walk on $G$ is recurrent.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Aldous-Broder algorithm](../../../combinatorics.md#aldous-broder-algorithm) starts the recurrent random walk at $x_0$ and, whenever it first visits a vertex $v\ne x_0$, adds the edge by which it entered $v$. Recurrence ensures that every vertex is eventually visited. The collection of first-entrance edges is a spanning tree and has the infinite-volume uniform spanning-tree law.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Fix a simple path of 2022 vertices in the first layer. The event that all its edges belong to the uniform spanning tree has positive probability: a finite acyclic edge set can be extended to a spanning tree in every sufficiently large finite exhaustion, and the transfer-current determinant for that forest has a positive infinite-volume limit.

The event that $T_1$ has a component of size at least 2022 is invariant under translations of $\mathbb Z^2$. The uniform spanning-tree law on this transitive recurrent graph is translation ergodic, so an invariant event of positive probability has probability one. Therefore $T_1$ almost surely has such a component.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The event that $T_1$ is connected is translation invariant and hence has probability zero or one. Layer-exchange symmetry gives the same probability for connectivity of $T_2$. If $T_1$ were connected almost surely, both induced forests would therefore be connected almost surely.

On that event the spanning tree must contain exactly one vertical edge: it needs at least one to join the two layers, while two vertical edges together with the unique paths inside the connected $T_1$ and $T_2$ would form a cycle. But a translation-invariant random set cannot contain exactly one vertical edge almost surely. Every specified vertical edge would have probability zero of being the unique one, and their countable union would still have probability zero. This contradiction proves that $T_1$ is almost surely not connected.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
