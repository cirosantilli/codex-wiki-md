# Paper 133

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20133.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20133.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
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

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Use the [Schreier coset graph](../../../geometric-group-theory.md#schreier-coset-graph) of the subgroup, with one directed edge labelled $s$ from $Hg$ to $Hgs$ for each $s\in\{a,b\}$. The homomorphism

$$
\phi:F_2\longrightarrow\mathbb Z,
\qquad
\phi(a)=1,\quad\phi(b)=0
$$

identifies the cosets of $\ker\phi$ with the integers. The covering graph therefore has vertices $v_n$, $n\in\mathbb Z$, an $a$-edge

$$
v_n\xrightarrow{\ a\ }v_{n+1}
$$

and a $b$-loop at every $v_n$. Thus it is a doubly infinite $a$-line with one $b$-circle attached at each integer vertex.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For

$$
\phi(a)=2,\qquad\phi(b)=3,
$$

the map $\phi:F_2\to\mathbb Z$ is surjective because $\gcd(2,3)=1$. Again identify the cosets of $\ker\phi$ with $\mathbb Z$. The covering has vertices $v_n$ and directed edges

$$
v_n\xrightarrow{\ a\ }v_{n+2},
\qquad
v_n\xrightarrow{\ b\ }v_{n+3}.
$$

This labelled graph is connected: integer combinations of $2$ and $3$ reach every vertex. Each vertex has one incoming and one outgoing edge of each label, as required for a [covering graph](../../../geometric-group-theory.md#covering-graph) of the two-petalled rose.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The based [Schreier coset graph](../../../geometric-group-theory.md#schreier-coset-graph) has vertices $\langle a\rangle g$ and an $s$-edge from $\langle a\rangle g$ to $\langle a\rangle gs$. At the base vertex $\langle a\rangle$ there is an $a$-loop. There are no other cycles: the fundamental group of the covering is the subgroup $\langle a\rangle\cong\mathbb Z$, and its displayed loop already generates it.

Equivalently, start with one $a$-circle at the base vertex and attach labelled trees so that every vertex has exactly one incoming and one outgoing $a$-edge and exactly one incoming and one outgoing $b$-edge. After deleting the base $a$-loop, the underlying graph is a tree. This describes the complete infinite covering and distinguishes it from its finite core, which is just the $a$-loop.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Whenever a combinatorial loop $\alpha$ traverses an oriented edge and immediately traverses the same edge backwards, delete that backtracking pair. Each deletion is a [homotopy relative to endpoints](../../../algebraic-topology.md#based-homotopy) inside $Z$ and reduces the edge length by two, so the process terminates at a reduced, hence locally injective, combinatorial loop $\beta$.

The universal cover $\widetilde Y$ of a connected graph is a [tree](../../../combinatorics.md#tree-graph-theory). The lift $\widetilde\beta$ is also locally injective because a [covering map](../../../algebraic-topology.md#covering-space) is a local graph isomorphism. A locally injective edge path in a tree cannot repeat a vertex: the segment between two successive visits would be a nonempty reduced closed path, whereas every closed path in a tree backtracks. Thus $\widetilde\beta$ is injective unless $\beta$ is constant.

Now let a loop in $Z$ become null-homotopic in $Y$. Its reduced representative $\beta$ lifts to a closed path in $\widetilde Y$. The preceding injectivity forces that lift, and hence $\beta$, to be constant. The original loop is null-homotopic in $Z$, proving that

$$
\pi_1(Z,y_0)\longrightarrow\pi_1(Y,y_0)
$$

is an injective [group homomorphism](../../../group-theory.md#group-homomorphism).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Choose a finite generating set $h_1,\ldots,h_r$ for $H$. Under the standard [classification of connected covering spaces](../../../algebraic-topology.md#classification-of-connected-covering-spaces), each $h_i$ is represented by a based combinatorial loop $\gamma_i$ in $Y$. Let $Z$ be the union of the images of these finitely many finite edge paths. Then $Z$ is a finite connected subgraph containing $y_0$.

Part (b) makes the inclusion-induced map

$$
\pi_1(Z,y_0)\longrightarrow\pi_1(Y,y_0)=H
$$

injective. Its image contains every $h_i$, because every $\gamma_i$ lies in $Z$, and therefore contains the subgroup they generate, namely all of $H$. The map is consequently an [isomorphism](../../../algebra.md#isomorphism).

## 2

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Write

$$
G=\langle u\rangle*_{\langle u^2\rangle=\langle v^3\rangle}\langle v\rangle.
$$

Its [Bass-Serre tree](../../../geometric-group-theory.md#bass-serre-tree) has vertices

$$
G/\langle u\rangle\ \sqcup\ G/\langle v\rangle
$$

and edges $G/C$, where $C=\langle u^2\rangle=\langle v^3\rangle$; the edge $gC$ joins $g\langle u\rangle$ to $g\langle v\rangle$. Since

$$
[\langle u\rangle:\langle u^2\rangle]=2,
\qquad
[\langle v\rangle:\langle v^3\rangle]=3,
$$

this is the infinite $(2,3)$-biregular tree: every $u$-type vertex has degree two and every $v$-type vertex has degree three.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The [HNN extension](../../../geometric-group-theory.md#hnn-extension) is the [Baumslag-Solitar group](../../../geometric-group-theory.md#baumslag-solitar-group)

$$
\operatorname{BS}(1,2)
=\langle u,t\mid tut^{-1}=u^2\rangle.
$$

Its [Bass-Serre tree](../../../geometric-group-theory.md#bass-serre-tree) has vertices $G/\langle u\rangle$ and oriented edges $G/\langle u\rangle$, with the two endpoint maps induced by the identity embedding and the index-two embedding $n\mapsto2n$. At each vertex there is one incident edge on the identity side and two on the index-two side. The underlying unoriented tree is therefore infinite and $3$-regular, with an orientation in which every vertex has one incoming and two outgoing edges, up to reversing the convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The relation is

$$
aba^{-1}=b^{-1},
$$

so $K$ is the [Klein bottle group](../../../geometric-group-theory.md#klein-bottle-group). Let it act on $\mathbb R^2$ by

$$
b(s,t)=(s+1,t),
\qquad
a(s,t)=(-s,t+1).
$$

These are [Euclidean isometries](../../../geometry-and-topology.md#rigid-transformation) and satisfy $aba^{-1}=b^{-1}$. Every element has a normal form $b^ma^n$. The orbit of $(0,0)$ is discrete, and a rectangle of finite size meets every orbit, so the action is proper and cocompact.

The square

$$
a^2(s,t)=(s,t+2)
$$

is a vertical translation, while $b$ is a horizontal translation. They commute, and

$$
(a^2)^m b^n=1
$$

as an isometry only when $m=n=0$. Hence $\langle a^2,b\rangle\cong\mathbb Z^2$. The normal form shows that every element lies in either $\langle a^2,b\rangle$ or $a\langle a^2,b\rangle$, so this subgroup has [index](../../../group.md#index-of-a-subgroup) two in $K$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Introduce $d=c^2$ and $e=a^2$. The two vertex groups

$$
A=\langle a,d\mid ada^{-1}=d^{-1}\rangle,
\qquad
B=\langle c,e\mid cec^{-1}=e^{-1}\rangle
$$

are [Klein bottle groups](../../../geometric-group-theory.md#klein-bottle-group). In $A$, the subgroup $\langle a^2,d\rangle$ is $\mathbb Z^2$ of index two; in $B$, the subgroup $\langle e,c^2\rangle$ is also $\mathbb Z^2$ of index two. Identifying

$$
e=a^2,\qquad d=c^2
$$

gives

$$
G\cong
A*_{\langle a^2,c^2\rangle}B.
$$

Eliminating $d,e$ from this [amalgamated free product](../../../algebraic-topology.md#amalgamated-free-product) recovers exactly the two given relators.

The [Bass-Serre tree](../../../geometric-group-theory.md#bass-serre-tree) is bipartite with vertex sets $G/A$ and $G/B$ and edge set $G/\langle a^2,c^2\rangle$. Both edge-group inclusions have index two, so every vertex has degree two. The tree is therefore a bi-infinite line, with $A$- and $B$-type vertices alternating.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Use the amalgam from part (c), with edge group

$$
C=\langle a^2,c^2\rangle.
$$

An odd power of $a$ belongs to $A\setminus C$, because $C$ is the index-two translation subgroup of the [Klein bottle group](../../../geometric-group-theory.md#klein-bottle-group) $A$. Similarly, an odd power of $c$ belongs to $B\setminus C$. Thus

$$
a^{i_1}c^{j_1}a^{i_2}\cdots c^{j_{n-1}}a^{i_n}c^{j_n}
$$

is a reduced alternating word whose syllables lie in $A\setminus C$ and $B\setminus C$. The [normal form theorem for an amalgamated free product](../../../geometric-group-theory.md#normal-form-theorem-for-an-amalgamated-free-product) says that every nonempty reduced alternating word is nonidentity. The displayed element is therefore nontrivial for every $n\geq1$.

## 3

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write the generators additively in the [abelianization](../../../group-theory.md#abelianization). The relators give

$$
x=2a,\qquad y=3b,\qquad c=-a-b,
$$

and

$$
7c+x+y=0.
$$

After substitution, the last relation becomes

$$
5a+4b=0.
$$

The commutator relators disappear automatically, so

$$
G^{\mathrm{ab}}\cong\mathbb Z^2/\langle(5,4)\rangle\cong\mathbb Z,
$$

because $\gcd(5,4)=1$. Explicitly, an isomorphism to $\mathbb Z$ sends

$$
\boxed{a\longmapsto4,\quad b\longmapsto-5,\quad
c\longmapsto1,\quad x\longmapsto8,\quad y\longmapsto-15.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let

$$
\Delta(2,3,7)
=\langle A,B,C\mid A^2=B^3=C^7=ABC=1\rangle
$$

be the orientation-preserving $(2,3,7)$ [hyperbolic triangle group](../../../geometric-group-theory.md#hyperbolic-triangle-group). Define

$$
a\mapsto A,\qquad b\mapsto B,\qquad c\mapsto C,
\qquad x\mapsto1,\qquad y\mapsto1.
$$

Every defining relator of $G$ maps to the identity, and $A,B,C$ lie in the image, so this is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism). Since

$$
\frac12+\frac13+\frac17<1,
$$

$\Delta(2,3,7)$ is a non-elementary [Fuchsian group](../../../geometric-group-theory.md#fuchsian-group).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The equality $x=a^2$ and the relator $[b,x]=1$ show that $x$ commutes with both $a$ and $b$. Since $c=(ab)^{-1}$, it also commutes with $c$, and then with $y=b^3$. Hence $x\in Z(G)$. Similarly, $y=b^3$ commutes with $b$ and, by $[a,y]=1$, with $a$; it therefore commutes with $c$ and $x$. Thus

$$
\langle x,y\rangle\leq Z(G).
$$

Quotienting by $\langle x,y\rangle$ gives

$$
G/\langle x,y\rangle
\cong\langle a,b,c\mid a^2,b^3,c^7,abc\rangle
=\Delta(2,3,7).
$$

A non-elementary [Fuchsian group](../../../geometric-group-theory.md#fuchsian-group) has trivial [center](../../../group-theory.md#center-of-a-group): two hyperbolic elements with different pairs of boundary fixed points have only the identity in their common centralizer in $\operatorname{PSL}_2(\mathbb R)$. Therefore the image in the quotient of every element of $Z(G)$ is trivial. It follows that

$$
\boxed{Z(G)=\langle x,y\rangle.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A hyperbolic [isometry of a tree](../../../geometric-group-theory.md#isometry-of-a-tree) has a unique invariant [axis of a tree isometry](../../../geometric-group-theory.md#axis-of-a-tree-isometry), on which it acts by a nonzero translation. Let $L$ be the axis of $x$. By part (c), $x$ is central, so for every $g\in G$,

$$
x(gL)=g(xL)=gL.
$$

**Thus $gL$ is another axis of $x$. Uniqueness gives $gL=L$, and hence the whole group $G$ preserves the line $L$.**

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $T^{Z(G)}$ be the common fixed subtree of the centre, which is nonempty by hypothesis and is $G$-invariant because $Z(G)$ is central. Restrict the action to this subtree. There $x$ and $y$ act pointwise trivially, so the action factors through

$$
G/\langle x,y\rangle\cong\Delta(2,3,7).
$$

In particular, the induced tree isometries satisfy

$$
a^2=b^3=c^7=1,\qquad abc=1.
$$

Assume, as usual for a combinatorial tree action, that edge inversions have been removed by barycentric subdivision. The finite-order elements $a,b,c$ are then [elliptic](../../../geometric-group-theory.md#elliptic-isometry-of-a-tree). Moreover

$$
ab=c^{-1},\qquad bc=a^{-1},\qquad ca=b^{-1},
$$

so each pairwise product is elliptic. [Serre lemma for tree actions](../../../geometric-group-theory.md#serre-lemma-for-tree-actions) implies that the fixed subtrees of each pair intersect. Convex subtrees of a tree have the [Helly property](../../../geometric-group-theory.md#helly-property), so

$$
\operatorname{Fix}(a)\cap\operatorname{Fix}(b)\cap\operatorname{Fix}(c)\ne\varnothing.
$$

Since $a,b,c$ generate $G/\langle x,y\rangle$, $G$ fixes a vertex of $T^{Z(G)}$. Thus the action of $G$ on $T$ is trivial in the tree-action sense.

## 4

↑ **Parent:** [Paper 133](paper-133.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $f:X\to T$ be a $(\lambda,\varepsilon)$-[quasi-isometry](../../../geometric-group-theory.md#quasi-isometry) to a tree. The image under $f$ of every geodesic segment in $X$ is a $(\lambda,\varepsilon)$-quasigeodesic in $T$. By the [Morse lemma for quasi-geodesics](../../../geometric-group-theory.md#morse-lemma-for-quasi-geodesics), it lies within a constant $R=R(\lambda,\varepsilon)$ of the tree geodesic with the same endpoints.

Consider a geodesic triangle in $X$. A point $p$ on one side maps within $R$ of the corresponding side of the comparison triangle in $T$. Every geodesic triangle in a tree is $0$-thin, so that comparison side is contained in the other two sides. Those two tree sides are in turn within $R$ of the images of the other two sides of the original triangle. Hence some point $q$ on one of those sides satisfies

$$
d_T(f(p),f(q))\leq2R.
$$

The lower quasi-isometry inequality gives

$$
d_X(p,q)\leq\lambda(2R+\varepsilon).
$$

**Thus $X$ is [Gromov-hyperbolic metric space](../../../geometric-group-theory.md#hyperbolic-metric-space) with $\delta=\lambda(2R+\varepsilon)$.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Retain the $(\lambda,\varepsilon)$-quasi-isometry $f:X\to T$ and the [Morse lemma for quasi-geodesics](../../../geometric-group-theory.md#morse-lemma-for-quasi-geodesics) constant $R$. Given $x,y\in X$, let $m$ be the midpoint of a geodesic $[x,y]$. There is a point $z$ on the tree geodesic $[f(x),f(y)]$ with

$$
d_T(f(m),z)\leq R.
$$

For any continuous path $\alpha$ from $x$ to $y$, choose a partition fine enough that consecutive $\alpha(t_i)$ are at distance at most one. Consecutive images under $f$ are then at distance at most

$$
D=\lambda+\varepsilon.
$$

Removing $z$ separates $f(x)$ from $f(y)$ in the tree along their geodesic, so this finite $D$-chain must contain an element within $D$ of $z$. For the corresponding $t_i$,

$$
d_T(f(m),f(\alpha(t_i)))\leq R+D.
$$

The lower quasi-isometry inequality yields

$$
d_X(m,\alpha(t_i))
\leq\lambda(R+D+\varepsilon).
$$

This constant depends only on the chosen quasi-isometry, so every [quasi-tree](../../../geometric-group-theory.md#quasi-tree) has the [bottleneck property](../../../geometric-group-theory.md#bottleneck-property).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [hyperbolic plane](../../../geometry-and-topology.md#hyperbolic-plane) $\mathbb H^2$ is a geodesic [Gromov-hyperbolic metric space](../../../geometric-group-theory.md#hyperbolic-metric-space) for some universal constant $\delta_0$. It is not a quasi-tree. Indeed, for every $C>0$, choose two points on opposite sides of a large closed metric ball centred at the midpoint of their joining geodesic. The complement of that ball in $\mathbb H^2$ is path connected, so the endpoints can be joined by a continuous path that stays more than $C$ from the midpoint. Thus $\mathbb H^2$ fails the [bottleneck property](../../../geometric-group-theory.md#bottleneck-property), whereas part (b) shows that every quasi-tree satisfies it.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Fix a hyperbolicity constant $\delta_0>0$ for $\mathbb H^2$. For a prescribed $\delta>0$, scale its distance by

$$
d_\delta=\frac{\delta}{\delta_0}d_{\mathbb H^2}.
$$

All distances in every geodesic triangle, including its thinness constant, scale by $\delta/\delta_0$. Hence

$$
X_\delta=(\mathbb H^2,d_\delta)
$$

is $\delta$-hyperbolic. Multiplication of a metric by a fixed positive constant is a [bilipschitz equivalence](../../../geometric-group-theory.md#bilipschitz-equivalence) and hence a [quasi-isometry](../../../geometric-group-theory.md#quasi-isometry). Therefore $X_\delta$ is quasi-isometric to $\mathbb H^2$ and cannot be a quasi-tree. This supplies an example for every $\delta>0$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
