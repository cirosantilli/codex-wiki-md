# Paper 111

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_111.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_111.pdf)

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
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [deletion condition for involutory generators](../../../lie-theory.md#deletion-condition-for-involutory-generators) says that whenever a word

$$
s_1s_2\cdots s_m,qquad s_i\in S,
$$

is not reduced, there are indices $i<j$ such that deleting $s_i$ and $s_j$ leaves a word representing the same group element.

The [exchange condition for a Coxeter group](../../../lie-theory.md#exchange-condition-for-a-coxeter-group) says that if $w=s_1\cdots s_m$ is reduced and $s\in S$ satisfies $\ell_S(sw)<\ell_S(w)$, then

$$
sw=s_1\cdots\widehat{s_i}\cdots s_m
$$

for some $i$. There is an equivalent right-handed form for $\ell_S(ws)<\ell_S(w)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Assume deletion. If $w=s_1\cdots s_m$ is reduced and $\ell(sw)<m$, then the word $s,s_1,\ldots,s_m$ is not reduced. Deletion removes two letters. It must remove the initial $s$: otherwise left cancellation by $s$ would give a word for $w$ shorter than $m$. Deleting $s$ and one $s_i$ gives the exchange condition.

Assume exchange, and suppose $sw$ and $wt$ are both ascents of $w$. Write $w=s_1\cdots s_m$ reduced. Then $s_1\cdots s_mt$ is reduced. If $swt$ is not a two-step ascent, left exchange deletes one letter from this expression. Deleting one of the $s_i$ would, after right cancellation by $t$, express $sw$ with at most $m-1$ letters, contradicting $\ell(sw)=m+1$. Thus exchange deletes the final $t$, and $swt=w$. This is the [folding condition](../../../lie-theory.md#folding-condition).

Finally assume folding. Consider a shortest counterexample to deletion and draw the array of lengths of all consecutive subwords $s_i\cdots s_j$. Adjacent entries differ by at most one because each generator is an involution. Starting at the first place where the full word fails to be geodesic and following the boundary between ascents and descents produces a square in which left and right multiplication are both ascents but the diagonal is not a two-step ascent. Folding identifies the opposite vertices of this square. Cancelling the common prefix and suffix says that two letters of the original word may be deleted. This contradicts the choice of a counterexample and proves deletion. This standard argument is the [folding-grid proof of the deletion condition](../../../lie-theory.md#folding-grid-proof-of-the-deletion-condition).

Hence

$$
\boxed{(D)\Longleftrightarrow(E)\Longleftrightarrow(F).}
$$

## 2

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Cayley graph](../../../geometric-group-theory.md#cayley-graph) $\operatorname{Cay}_S(W)$ has vertex set $W$ and an unoriented edge $\{w,ws\}$ for every $w\in W$ and $s\in S$.

For a [reflection of a Coxeter group](../../../lie-theory.md#reflection-of-a-coxeter-group) $r\in R$, its wall is

$$
H_r=\bigl\{\{w,ws\}:wsw^{-1}=r\bigr\}.
$$

Equivalently, these are the edges fixed setwise and reversed by left multiplication by $r$. Removing their interiors separates the Cayley graph into two [half-spaces](../../../lie-theory.md#half-space-of-a-coxeter-group).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $w=s_1\cdots s_m$ be reduced and follow the corresponding geodesic from $e$ to $w$. Its $i$th edge belongs to the wall of

$$
r_i=s_1\cdots s_{i-1}s_i s_{i-1}\cdots s_1.
$$

A reduced path crosses each wall at most once, and these $m$ walls are exactly the walls separating its endpoints. Moreover

$$
r_iw=s_1\cdots\widehat{s_i}\cdots s_m,
$$

so $\ell(r_iw)<\ell(w)$. Conversely, if $\ell(rw)<\ell(w)$, write $r=usu^{-1}$ and apply the [exchange condition for a Coxeter group](../../../lie-theory.md#exchange-condition-for-a-coxeter-group) to a reduced expression: it identifies $r$ with one of the reflections $r_i$. Therefore

$$
\boxed{H_r\text{ separates }e\text{ from }w
\iff \ell(rw)<\ell(w).}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

By part (b), the hypothesis says that every wall separates $e$ from $w_0$. Let $u\in W$. For each wall, $e$ and $w_0$ lie in opposite half-spaces, so $u$ lies on exactly one of their two sides. The wall therefore separates exactly one of the pairs $(e,u)$ and $(u,w_0)$. Since Coxeter length equals the number of separating walls,

$$
\boxed{\ell(w_0)
=|\mathcal H(e,w_0)|
=|\mathcal H(e,u)|+|\mathcal H(u,w_0)|
=\ell(u)+\ell(u^{-1}w_0).}
$$

## 3

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Restrict the Coxeter matrix of $(W,S)$ to $T\times T$ and let $W'$ be the Coxeter group defined by that matrix. Sending its generators to the corresponding elements of $T$ gives a surjection $W'\to W_T$. The [Geometric representation of a Coxeter group](../../../lie-theory.md#geometric-representation-of-a-coxeter-group) for $W'$ is the restriction of the geometric representation for $W$ to the span of the simple roots indexed by $T$. Faithfulness of the geometric representation makes the map injective. Hence

$$
\boxed{(W_T,T)\text{ is a Coxeter system}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Part (a) gives a reduced $T$-word for $w$. It is also reduced as an $S$-word, since a shorter $S$-word would contradict the length function obtained from the restricted geometric representation. By [Matsumoto theorem](../../../lie-theory.md#matsumoto-theorem), this expression and the given reduced expression $s_1\cdots s_k$ differ by braid moves. Every braid move starting with letters in $T$ replaces them by the same two letters in the opposite alternating order, so it never introduces a generator outside $T$. Therefore every $s_i$ lies in $T$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

By part (a), every full subdiagram gives a standard parabolic Coxeter subgroup. In the $B_{n+1}$ diagram, the $n$ vertices away from the endpoint incident to the edge labelled four form an $A_n$ chain. Thus

$$
W(A_n)\subset W(B_{n+1}).
$$

The $E_8$ diagram is a trivalent tree whose three arms have lengths $1,2,4$ beyond the central vertex. Removing the endpoint of the arm of length one leaves a chain of seven vertices, hence an $A_7$ subdiagram. Removing the outer endpoint of the arm of length two leaves arms of lengths $1,1,4$, the $D_7$ diagram. Consequently

$$
\boxed{W(A_7)\subset W(E_8),
\qquad W(D_7)\subset W(E_8).}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Realize the generators as affine reflections of $\mathbb R^2$:

$$
s(x,y)=(-x,y),
\qquad
u(x,y)=(x,-y),
\qquad
t(x,y)=(1-y,1-x).
$$

The reflecting lines for $s$ and $u$ are perpendicular, while the line $x+y=1$ meets each at angle $\pi/4$. Hence

$$
s^2=t^2=u^2=(su)^2=(st)^4=(tu)^4=1,
$$

so the presentation maps onto this affine reflection group. But

$$
g=sut,qquad g(x,y)=(y-1,x-1),qquad
g^2(x,y)=(x-2,y-2),
$$

and $g$ has infinite order. Thus $W$ is infinite. The finite Coxeter group $W(B_4)$ is the [signed symmetric group](../../../lie-theory.md#hyperoctahedral-group) on four letters and has order $2^4 4!$. An infinite group cannot embed in it, so $W$ is not a subgroup of $W(B_4)$.

## 4

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Here $W=\langle s,t:s^2=t^2=(st)^2=1\rangle\cong C_2\times C_2$. In the [Davis complex](../../../lie-theory.md#davis-complex) described by the [basic construction of a Coxeter group](../../../lie-theory.md#basic-construction-of-a-coxeter-group), the fundamental chamber $K$ is the order complex of

$$
\varnothing,\quad\{s\},\quad\{t\},\quad\{s,t\};
$$

it consists of two triangles sharing the edge from $\varnothing$ to $\{s,t\}$. Four labelled copies $wK$ are glued along their $s$- and $t$-mirrors. The result is a square subdivided from its centre to the midpoints and vertices of its boundary, with eight triangular chambers.

For the poset description, the spherical cosets consist of four singleton cosets $wW_\varnothing$, four cosets of rank-one parabolics, and the single coset $W_{\{s,t\}}=W$. Their flag realization has one vertex at each original square vertex, one at each edge midpoint, and one at the square centre; its flags are precisely the same eight triangles. Thus the two requested drawings are the chamber-gluing picture and the barycentric subdivision of a square, respectively.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write the basic construction as

$$
U(W,K)=(W\times K)/\sim,
$$

where $(w,x)\sim(w',x)$ exactly when $w^{-1}w'$ belongs to the subgroup generated by the mirrors containing $x$. Let $v_T$ be the vertex of $K$ corresponding to a [spherical subset of a Coxeter system](../../../lie-theory.md#spherical-subset-of-a-coxeter-system) $T$. Its stabilizer is $W_T$. Therefore

$$
\operatorname{Stab}_W([w,v_T])
=wW_Tw^{-1}.
$$

Every conjugate of every spherical standard parabolic subgroup consequently occurs as a vertex stabilizer.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Order the chambers $wK$ by nondecreasing [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length), beginning with $K$. When $wK$ is attached, let

$$
T(w)=\{s\in S:\ell(ws)<\ell(w)\}
$$

be its right descent set. Claim C2 applied to the coset $wW_{T(w)}$, followed by C1, shows that $T(w)$ is spherical. The part of $wK$ already present is exactly

$$
wK^{T(w)}=w\bigcup_{s\in T(w)}K_s.
$$

It is nonempty for $w\ne e$ and is contractible by C3. The chamber $wK$ is contractible as well, so C4 shows inductively that every finite length-ordered union of chambers is contractible.

The Davis complex is a [CW complex](../../../algebraic-topology.md#cw-complex) and is the increasing union of these chamber unions. Every map from a sphere has compact image and therefore lies in a finite union; the next finite contractible union null-homotopes it. Thus every homotopy group of the Davis complex vanishes. Since it is connected, the [Whitehead theorem](../../../algebraic-topology.md#whitehead-theorem) implies

$$
\boxed{\Sigma(W,S)\text{ is contractible}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
