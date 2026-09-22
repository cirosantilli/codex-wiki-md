# Paper 134

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_134.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_134.pdf)

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

## 1

↑ **Parent:** [Paper 134](paper-134.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a finite [graph](../../../graph.md) $\Gamma$, its [Right-angled Artin group](../../../geometric-group-theory.md#right-angled-artin-group) is

$$
A_\Gamma=\left\langle v\in V(\Gamma)\mathrel{\middle|}[v,w]=1\text{ for every }\{v,w\}\in E(\Gamma)\right\rangle.
$$

Its [Salvetti complex](../../../geometric-group-theory.md#salvetti-complex) $S_\Gamma$ is the one-vertex [cube complex](../../../geometric-group-theory.md#cubical-complex) with an oriented loop labelled $v$ for each vertex of $\Gamma$, a square torus for every edge, and more generally one cubulated $k$-torus for every $k$-clique, attached compatibly along coordinate subtori. Thus $\pi_1(S_\Gamma)\cong A_\Gamma$. The [vertex link of a Salvetti complex](../../../geometric-group-theory.md#vertex-link-of-a-salvetti-complex) is flag, so $S_\Gamma$ is a [nonpositively curved cube complex](../../../geometric-group-theory.md#nonpositively-curved-cube-complex).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

If $\Gamma=\Gamma_1\sqcup\Gamma_2$ is a nontrivial [disjoint union of graphs](../../../graph-theory.md#disjoint-union-of-graphs), no defining relation mixes the two vertex sets, and hence

$$
A_\Gamma\cong A_{\Gamma_1}*A_{\Gamma_2}.
$$

On the topological side, every clique lies in one component, so

$$
S_\Gamma=S_{\Gamma_1}\vee S_{\Gamma_2},
$$

a one-point union of [Salvetti complexes](../../../geometric-group-theory.md#salvetti-complex).

If $\Gamma=\Gamma_1*\Gamma_2$ is a nontrivial [join of graphs](../../../graph-theory.md#join-graph-theory), every generator from the first part commutes with every generator from the second. Therefore

$$
A_\Gamma\cong A_{\Gamma_1}\times A_{\Gamma_2}.
$$

Every clique of the join is the union of a clique in each factor, which gives the cubical identity

$$
\boxed{S_\Gamma\cong S_{\Gamma_1}\times S_{\Gamma_2}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For each $v\in V(\Gamma)$, the [vertex link of a Salvetti complex](../../../geometric-group-theory.md#vertex-link-of-a-salvetti-complex) has two vertices $v^+$ and $v^-$. If $v$ has degree $d_\Gamma(v)$, then each of $v^+$ and $v^-$ is adjacent to both signed vertices $w^+,w^-$ for every neighbour $w$, and hence has link degree $2d_\Gamma(v)$.

Suppose the whole link is a cycle. Every link vertex has degree two, so every vertex of $\Gamma$ has degree one. The link is connected, which forces $\Gamma$ to be connected. A connected one-regular graph consists of one edge. Conversely, if $\Gamma$ is one edge, then $S_\Gamma$ is the square [torus](../../../topology.md#torus) and its unique vertex has link the four-cycle

$$
v^+\ {-}\ w^+\ {-}\ v^-\ {-}\ w^-\ {-}\ v^+.
$$

**Thus the vertex link is a cycle exactly when $\Gamma$ is an edge.**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [hyperplane of a Salvetti complex](../../../geometric-group-theory.md#hyperplane-of-a-salvetti-complex) dual to the loop labelled $v$ is itself the Salvetti complex of the [induced subgraph](../../../graph-theory.md#induced-subgraph) on the neighbours of $v$. If this hyperplane were homeomorphic to a closed surface, its vertex link would be a cycle. Part (c), applied to that induced graph, says that the graph must be one edge. Its Salvetti complex is therefore the two-dimensional [torus](../../../topology.md#torus), a surface of genus one. It cannot be a [closed orientable surface](../../../topology.md#closed-orientable-surface) of genus two.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The inclusion of a [full subgraph](../../../graph-theory.md#induced-subgraph) $\Gamma'\subseteq\Gamma$ sends each generator of $A_{\Gamma'}$ to the equally named generator of $A_\Gamma$. Define

$$
r:A_\Gamma\longrightarrow A_{\Gamma'}
$$

by fixing the generators in $\Gamma'$ and sending every other generator to the identity. Every commutator relation of $A_\Gamma$ maps to a valid relation, so $r$ is a [group homomorphism](../../../group-theory.md#group-homomorphism). Its composite with the natural map $A_{\Gamma'}\to A_\Gamma$ is the identity. The natural map has a left inverse and is therefore injective, proving that $A_{\Gamma'}$ is isomorphic to a subgroup of $A_\Gamma$.

## 2

↑ **Parent:** [Paper 134](paper-134.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A group is cubulated when it admits a [cubulation of a group](../../../geometric-group-theory.md#cubulation-of-a-group), namely a [metrically proper group action](../../../geometric-group-theory.md#metrically-proper-group-action) by cubical automorphisms on a [CAT(0) cube complex](../../../geometric-group-theory.md#cat-0-cube-complex). It is cocompactly cubulated when that action is also a [cocompact group action](../../../geometric-group-theory.md#cocompact-group-action). Thus a cocompact cubulation is a proper, cocompact cubical action.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix $x\in S$ and let $\sigma_x$ be its [principal vertex of a dual cube complex](../../../geometric-group-theory.md#principal-vertex-of-a-dual-cube-complex). The combinatorial distance in the dual complex is the [wall metric](../../../geometric-group-theory.md#wall-metric):

$$
d_C(\sigma_x,g\sigma_x)
=d_{\mathcal W}(x,gx)
=\#\{W\in\mathcal W:W\text{ separates }x\text{ from }gx\}.
$$

Consequently the [wall-metric properness criterion](../../../geometric-group-theory.md#wall-metric-properness-criterion) says that the action on $C$ is metrically proper provided this number tends to infinity as $g$ leaves every finite subset of $G$. Equivalently, for every $R$, only finitely many $g$ separate $x$ from $gx$ by at most $R$ walls.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The necessary and sufficient condition is the [transverse-wall cocompactness criterion](../../../geometric-group-theory.md#transverse-wall-cocompactness-criterion): there must be finitely many $G$-orbits of finite [transverse wall collections](../../../geometric-group-theory.md#transverse-wall-collection). Equivalently, their cardinalities must be uniformly bounded and, for every cardinality, there must be only finitely many orbits.

Indeed, an $n$-cube of the [dual cube complex of a wallspace](../../../geometric-group-theory.md#dual-cube-complex-of-a-wallspace) is dual to an $n$-element collection of pairwise crossing walls, and this correspondence respects the $G$-action and passage to faces. If there are finitely many orbits of transverse collections, there are finitely many cube orbits, so the quotient $G\backslash C$ is a finite cube complex and is compact. Conversely, if the action is cocompact, a compact fundamental set meets only finitely many open unit cubes. Hence there are finitely many cube orbits and therefore finitely many orbits of their dual transverse wall collections.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The walls occur in three families of parallel lines, and a choice of halfspaces in one family is determined by an integer cut. Lines from different families cross, so the three cuts can be chosen independently. It follows directly from the [dual cube complex of a wallspace](../../../geometric-group-theory.md#dual-cube-complex-of-a-wallspace) construction that

$$
C^{(0)}\cong\mathbb Z^3
$$

and that $C$ is the standard cubulation of $\mathbb R^3$.

Choose affine coordinates $x_1,x_2,x_3$ for the three wall families so that the original Euclidean plane is $x_1+x_2+x_3=0$ and the walls are the integer level sets. On the cut coordinates $(n_1,n_2,n_3)\in\mathbb Z^3$, the translation subgroup of the [Affine Coxeter group](../../../lie-theory.md#affine-coxeter-group) $W$ adds vectors $(m_1,m_2,m_3)$ satisfying $m_1+m_2+m_3=0$, while its finite reflection subgroup permutes the three coordinates. Therefore

$$
h(n_1,n_2,n_3)=n_1+n_2+n_3
$$

is constant on every $W$-orbit. Since $h(n,0,0)=n$ is unbounded, there are infinitely many vertex orbits. A cocompact cubical action on this locally finite cube complex would have only finitely many cube orbits, so the action of $W$ on $C$ is not cocompact.

## 3

↑ **Parent:** [Paper 134](paper-134.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A group $G$ is [residually finite](../../../group-theory.md#residually-finite-group) if, for every $1\ne g\in G$, there are a finite group $Q$ and a homomorphism $\phi:G\to Q$ such that $\phi(g)\ne1$.

Let $F(S)$ be a [free group](../../../geometric-group-theory.md#free-group) and let $1\ne w\in F(S)$ be a reduced word. In the rose with one oriented loop for each $s\in S$, the word $w$ determines a nonclosed reduced path from a chosen vertex in the universal covering tree. Its finite image path can be completed to a finite [covering graph](../../../geometric-group-theory.md#covering-graph) of the rose: for each label, pair the still unmatched incoming and outgoing edge germs, adding finitely many vertices if necessary. The lift of $w$ remains nonclosed in this finite cover.

Let $H\le F(S)$ be the finite-index subgroup represented by this based cover. Then $w\notin H$. The action of $F(S)$ on the finite set of right cosets $H\backslash F(S)$ gives a homomorphism to a finite [symmetric group](../../../finite-group-theory.md#symmetric-group), and $w$ does not fix the coset $H$. Thus $w$ survives in a finite quotient. Since $w$ was arbitrary, every free group is residually finite.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $X$ be a subcomplex of a product of graphs $A\times B$. Orient every edge of each factor. An edge of $X$ is horizontal or vertical according to its factor, and this type is preserved across opposite sides of every square.

A [hyperplane of a cube complex](../../../geometric-group-theory.md#hyperplane-of-a-cube-complex) of horizontal type retains one fixed edge of $A$ while moving through edges of $B$; the analogous statement holds vertically. The factor orientation makes every hyperplane two-sided. A square has one horizontal and one vertical direction, so no hyperplane self-intersects. At a vertex there is at most one incident edge with a fixed factor edge and orientation, so no hyperplane self-osculates. Finally, a horizontal hyperplane and a vertical hyperplane can cross only in the unique product square determined by their two factor edges. If that square belongs to $X$, it fills every corner at which those two dual edges meet; if it does not, the hyperplanes never cross. Thus no pair interosculates. All four hyperplane pathologies are absent, so $X$ is a [special cube complex](../../../geometric-group-theory.md#special-cube-complex).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Call the two horizontal edge classes indicated by one and two arrowheads $a$ and $b$. All vertices in the displayed quotient are identified. In the third displayed square, an $a$-edge and a $b$-edge are opposite, so they are dual to the same [hyperplane of a cube complex](../../../geometric-group-theory.md#hyperplane-of-a-cube-complex) $H$. At the unique vertex, the distinct edges $a$ and $b$ are therefore dual to $H$, but no square has them as adjacent sides. With the orientations shown, they have the same initial vertex. Hence $H$ is a [self-osculating hyperplane](../../../geometric-group-theory.md#self-osculating-hyperplane), one of the forbidden pathologies of a [special cube complex](../../../geometric-group-theory.md#special-cube-complex). The displayed cube complex is not special.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Because $X$ is special, the [fundamental group of a special cube complex](../../../geometric-group-theory.md#fundamental-group-of-a-special-cube-complex) embeds in a [Right-angled Artin group](../../../geometric-group-theory.md#right-angled-artin-group). Right-angled Artin groups are residually finite by the [residual finiteness of a right-angled Artin group](../../../geometric-group-theory.md#residual-finiteness-of-a-right-angled-artin-group), and a [subgroup of a residually finite group](../../../group-theory.md#subgroup-of-a-residually-finite-group) is residually finite. Hence $\pi_1X$ is residually finite.

If $\pi_1X$ were simple, choose $1\ne g\in\pi_1X$. A finite quotient in which $g$ survives has a proper normal kernel. Simplicity would force that kernel to be trivial, embedding $\pi_1X$ into a finite group, contrary to the assumption that $\pi_1X$ is infinite. This is precisely the obstruction that an [infinite residually finite group is not simple](../../../group-theory.md#infinite-residually-finite-group-is-not-simple).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
