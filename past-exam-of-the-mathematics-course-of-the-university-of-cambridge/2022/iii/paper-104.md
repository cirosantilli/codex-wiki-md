# Paper 104

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_104.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_104.pdf)

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
    - [1](#2/a/1)
      - [Solution](#2/a/1/solution)
    - [2](#2/a/2)
      - [Solution](#2/a/2/solution)
    - [3](#2/a/3)
      - [Solution](#2/a/3/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 104](paper-104.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Because the generating sets are disjoint, the [free product](../../../algebraic-topology.md#free-product) has the presentation

$$
\boxed{G*H=\langle X\sqcup Y\mid R\sqcup S\rangle.}
$$

This is immediate from the [universal property of a group presentation](../../../geometric-group-theory.md#universal-property-of-a-group-presentation): a map out of this presented group is exactly a pair of homomorphisms from $G$ and $H$ to the target group.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A reduced word is either the empty word or a product

$$
u_1u_2\cdots u_n
$$

in which every syllable $u_i$ is a nonidentity element of $G$ or $H$, and consecutive syllables belong to different factors.

Let $\mathcal W$ be the set of reduced words. Each $g\in G$ acts on the right of $\mathcal W$: if the last syllable lies in $H$, append $g$; if it lies in $G$, multiply it by $g$ and delete it when the product is the identity. Define the action of each $h\in H$ analogously. These rules give genuine actions of the two factors by [permutations](../../../combinatorics.md#permutation) of $\mathcal W$, hence an action of the [free group](../../../geometric-group-theory.md#free-group) $F(X\sqcup Y)$. Every relation in $R\sqcup S$ acts trivially, so the action factors through the displayed presentation of $G*H$.

The element represented by a reduced word $w$ sends the empty word to $w$. Therefore two reduced words representing the same element induce the same permutation and have the same value on the empty word. They must be identical. This proves the [normal form theorem for a free product](../../../algebraic-topology.md#normal-form-theorem-for-a-free-product).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $w$ be a nonempty reduced word. If its first syllable belongs to $G$, choose any nonidentity $h\in H$. The reduced form of $hw$ begins with an $H$-syllable, whereas that of $wh$ begins with the original $G$-syllable; reduction at the right end cannot change the first syllable. Hence $hw\ne wh$. The same argument with a nonidentity $g\in G$ applies when $w$ begins in $H$. No nonidentity element is therefore central, and

$$
\boxed{Z(G*H)=1.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Choose distinct nonidentity elements $g_1,g_2\in G$ and $h_1,h_2\in H$, and put

$$
u=g_1h_1,
\qquad
v=g_2h_2.
$$

Expand a freely reduced word in $u^{\pm1},v^{\pm1}$. At a boundary where two syllables from one factor meet, their product is one of $g_1^{-1}g_2$, $g_2^{-1}g_1$, $h_1h_2^{-1}$, or $h_2h_1^{-1}$, all nonidentity by the choices above. Every other boundary already alternates between the factors. Thus the expansion reduces to a nonempty reduced word in $G*H$ and cannot represent the identity. The homomorphism from the rank-two [free group](../../../geometric-group-theory.md#free-group) sending its free generators to $u,v$ is injective, so

$$
\boxed{\langle u,v\rangle\cong F_2.}
$$

## 2

↑ **Parent:** [Paper 104](paper-104.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/1">1</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/1/solution">Solution</h5>

↑ **Parent:** [1](#2/a/1)

The [Integer Heisenberg group](../../../lie-algebra.md#integer-heisenberg-group)

$$
H_3(\mathbb Z)=
\left\{
\begin{pmatrix}1&a&c\\0&1&b\\0&0&1\end{pmatrix}:a,b,c\in\mathbb Z
\right\}
$$

is generated by the matrices with $(a,b,c)=(1,0,0)$ and $(0,1,0)$. Their [group commutator](../../../group.md#group-commutator) is the nonidentity central matrix with $(a,b,c)=(0,0,1)$. Thus it is nonabelian and [nilpotent](../../../group-theory.md#nilpotent-group) of class two, while being finitely generated.

<h4 id="2/a/2">2</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/2/solution">Solution</h5>

↑ **Parent:** [2](#2/a/2)

The countable direct sum

$$
\bigoplus_{n\geq0}\mathbb Z
$$

is abelian and therefore nilpotent of class one. It is not finitely generated, whereas every [polycyclic group](../../../group-theory.md#polycyclic-group) is finitely generated. Hence it is nilpotent but not polycyclic.

<h4 id="2/a/3">3</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/3/solution">Solution</h5>

↑ **Parent:** [3](#2/a/3)

The [lamplighter group](../../../group-theory.md#lamplighter-group)

$$
C_2\wr\mathbb Z=\left(\bigoplus_{n\in\mathbb Z}C_2\right)\rtimes\mathbb Z
$$

is generated by one lamp switch and one translation. It is [metabelian](../../../group-theory.md#metabelian-group), hence solvable. Its base subgroup $\bigoplus_{\mathbb Z}C_2$ is not finitely generated. Every subgroup of a polycyclic group is finitely generated, so the lamplighter group is not polycyclic.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $N$ be the subgroup whose upper-left block is $I_2$. It is a finitely generated nilpotent subgroup of the integer [upper unitriangular group](../../../finite-group-theory.md#upper-unitriangular-group) $UT_4(\mathbb Z)$ and is normal in $L$. The block-diagonal matrix

$$
t=\operatorname{diag}(A,I_2)
$$

generates an infinite cyclic quotient, so

$$
L=N\rtimes\langle t\rangle.
$$

Finitely generated nilpotent groups are polycyclic, and an extension of polycyclic groups is polycyclic. Hence $L$ is polycyclic.

Inside $L$, retain only $t$ and the entries in positions $(1,3)$ and $(2,3)$. They form a subgroup

$$
\mathbb Z^2\rtimes_A\mathbb Z.
$$

The characteristic polynomial of $A$ is $\lambda^2-5\lambda+1$, so its eigenvalues are

$$
\frac{5\pm\sqrt{21}}2.
$$

One has modulus greater than one, and the resulting semidirect product has [exponential growth](../../../group-theory.md#exponential-growth-of-a-group). Every finitely generated virtually nilpotent group has polynomial growth, as does each of its finitely generated subgroups. Therefore $L$ cannot be virtually nilpotent.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 104](paper-104.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The empty word is the unique vertex of degree three in the underlying [tree](../../../combinatorics.md#tree-graph-theory); every other vertex has degree four. Every graph automorphism therefore fixes the empty word and permutes its three neighbours. Those neighbours are precisely $\{\mathbf0,\mathbf1,\mathbf2\}$, so this set is invariant.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The automorphism $a$ cyclically permutes the first letter and leaves the remaining suffix unchanged, so $a^3=1$ and $a\ne1$.

In the [section](../../../combinatorics.md#section-of-a-rooted-tree-automorphism) notation,

$$
b=(a,1,b).
$$

Thus $b^3=(a^3,1,b^3)=(1,1,b^3)$. An automorphism $c$ satisfying $c=(1,1,c)$ fixes every finite word: repeatedly entering the third subtree eventually reaches the end of the word. Hence $b^3=1$. Since $b(\mathbf{00})=\mathbf{01}$, it is nonidentity, and both $a$ and $b$ have order three.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The action on the first level defines a surjective homomorphism

$$
G\longrightarrow\langle(\mathbf0\,\mathbf1\,\mathbf2)\rangle\cong C_3
$$

that sends $a$ to the displayed cycle and $b$ to the identity. Its kernel is therefore the normal closure of $b$, proving that $\{b\}$ normally generates $\operatorname{Stab}_G(1)$.

Apply the [Reidemeister–Schreier theorem](../../../geometric-group-theory.md#reidemeister-schreier-theorem) with transversal $\{1,a,a^{-1}\}$. The generators arising from $a$ are trivial, while those arising from $b$ are

$$
b,qquad aba^{-1},qquad a^{-1}ba.
$$

**Consequently these three elements generate $\operatorname{Stab}_G(1)$.**

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

An element $g$ fixing the first level restricts to an automorphism $g_i$ on each rooted subtree, and composition is coordinatewise. Therefore

$$
\phi(g)=(g_0,g_1,g_2)
$$

is a homomorphism. If all three sections are trivial, $g$ fixes every word, so $\phi$ is injective.

Directly from the recursions,

$$
\phi(b)=(a,1,b),qquad
\phi(aba^{-1})=(b,a,1),qquad
\phi(a^{-1}ba)=(1,b,a).
$$

The generators found in the preceding part therefore have every section in $G$, so $\phi(\operatorname{Stab}_G(1))\subseteq G^3$.

Moreover, every coordinate projection of this image contains both $a$ and $b$, and is therefore onto $G$. Since $a$ acts transitively on the first level, induction shows that $G$ acts transitively on every level of the [rooted tree](../../../combinatorics.md#rooted-tree). The $n$th level has $3^n$ vertices, so the orders of these finite orbits are unbounded. Hence $G$ is infinite.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Use the convention $[g,h]=g^{-1}h^{-1}gh$. In $G/K$ the images of $a$ and $b$ commute and both have order three, so $G/K$ is a quotient of $C_3\times C_3$. Thus

$$
[G:K]\leq9.
$$

Put $d=a^{-1}ba$. From the preceding section calculations,

$$
\phi(d)=(1,b,a),qquad
\phi(x)=\phi([a,b])=(a,b^{-1},a^{-1}b).
$$

Since both elements fix the first level, their commutator is computed coordinatewise, and

$$
\phi([d,x])=(1,1,x).
$$

The element $[d,x]$ belongs to $K$. The third-coordinate projection of $\phi(\operatorname{Stab}_G(1))$ is onto $G$, so conjugating this element inside the stabilizer shows that $\phi(K)$ contains $(1,1,x^g)$ for every $g\in G$. Because the conjugates $x^g$ generate $K$, it contains $1\times1\times K$. Conjugation by $a$ cyclically permutes the coordinates; hence it also contains $K\times1\times1$ and $1\times K\times1$. These coordinate subgroups commute, giving

$$
\boxed{K\times K\times K\ leq\phi(K\cap\operatorname{Stab}_G(1)).}
$$

Injectivity of $\phi$ identifies its inverse image with a subgroup of $K$ isomorphic to $K^3$.

## 4

↑ **Parent:** [Paper 104](paper-104.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A group $G$ is [residually finite](../../../group-theory.md#residually-finite-group) when, for every $1\ne g\in G$, there are a [finite group](../../../group.md#finite-group) $Q$ and a [group homomorphism](../../../group-theory.md#group-homomorphism) $q:G\to Q$ such that $q(g)\ne1$. Equivalently, the intersection of all finite-index normal subgroups of $G$ is trivial.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

By the [Fundamental theorem of finitely generated abelian groups](../../../group.md#fundamental-theorem-of-finitely-generated-abelian-groups),

$$
A\cong\mathbb Z^r\oplus T
$$

with $T$ finite. If a nonzero element has a nonzero component in $T$, projection to $T$ separates it. Otherwise some integer coordinate is a nonzero $n$; choose a prime $p$ not dividing $n$ and reduce that coordinate modulo $p$. This gives a finite quotient in which the element survives, so every finitely generated abelian group is residually finite.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

If $G$ is generated by $d$ elements, a homomorphism $G\to Q$ is determined by the images of those generators. There are at most $|Q|^d$ such choices, so only finitely many homomorphisms exist.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $\alpha:G\to G$ be surjective and suppose that $1\ne g\in\ker\alpha$. By residual finiteness, choose $q:G\to Q$ with $Q$ finite and $q(g)\ne1$. The preceding part makes the sequence

$$
q,\ q\alpha,\ q\alpha^2,\ldots
$$

repeat, so $q\alpha^i=q\alpha^j$ for some $i<j$. Surjectivity of $\alpha^i$ permits cancellation on the right and gives $q=q\alpha^{j-i}$. But $g\in\ker\alpha^{j-i}$, which would imply $q(g)=1$, a contradiction. Thus $\alpha$ is injective. Every finitely generated residually finite group is therefore a [Hopfian group](../../../group-theory.md#hopfian-group).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Enumerate $X=\{x_1,\ldots,x_n\}$ and $Y=\{y_1,\ldots,y_n\}$. The [universal property of a free group](../../../geometric-group-theory.md#universal-property-of-a-free-group) gives an endomorphism

$$
\alpha:F(X)\longrightarrow F(X),qquad \alpha(x_i)=y_i.
$$

Since $Y$ generates, $\alpha$ is surjective. The finitely generated free group is residually finite and hence Hopfian by the preceding part, so $\alpha$ is an automorphism. An automorphism sends a free basis to a free basis; therefore $Y$ is a basis of $F(X)$.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

For the free basis $X=\{x_0,x_1,x_2,\ldots\}$, define

$$
\alpha(x_0)=1,
\qquad
\alpha(x_{n+1})=x_n.
$$

The [universal property of a free group](../../../geometric-group-theory.md#universal-property-of-a-free-group) extends this assignment to an endomorphism of $F(X)$. It is surjective because every $x_n$ is the image of $x_{n+1}$, but it is not injective because $x_0\ne1$ lies in its kernel. Thus $F(\mathbb N)$ is not Hopfian.

## 5

↑ **Parent:** [Paper 104](paper-104.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let

$$
B=\bigoplus_{g\in G}H_g
$$

be the group of finitely supported functions $f:G\to H$ with pointwise multiplication. The left-translation action

$$
(g\cdot f)(x)=f(g^{-1}x)
$$

defines the restricted [wreath product](../../../group-theory.md#wreath-product)

$$
\boxed{H\wr G=B\rtimes G.}
$$

Suppose $X$ and $Y$ are finite generating sets for $G$ and $H$. Embed each $y\in Y$ as a lamp supported at the identity of $G$. Conjugating these lamps by words in $X$ produces copies of $Y$ at every coordinate, and these copies generate $B$. Thus $X$ together with the identity-coordinate copy of $Y$ is a finite generating set for $H\wr G$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $\theta:H\wr G\to Q$ be any homomorphism to a finite group. Because $G$ is infinite, two distinct elements $r,s\in G$ have $\theta(r)=\theta(s)$. For $h\in H$, denote by $h_g$ the lamp with value $h$ at $g$. Conjugation translates lamps, so

$$
\theta(h_r)=\theta(h_s)
$$

for every $h\in H$. Choose $h,k\in H$ with $[h,k]\ne1$. Lamps at different coordinates commute, and therefore

$$
\theta([h_r,k_r])
=\theta([h_s,k_r])=1.
$$

But $[h_r,k_r]$ is the nonidentity lamp $[h,k]_r$. This same nonidentity element is killed by every finite quotient, so $H\wr G$ is not residually finite.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Choose $1\ne h\in H$ and let $t$ generate $\mathbb Z$. For each binary string $(\varepsilon_0,\ldots,\varepsilon_{n-1})$, the word

$$
h^{\varepsilon_0}t h^{\varepsilon_1}t\cdots t h^{\varepsilon_{n-1}}t^{-(n-1)}
$$

records that string in the lamps at positions $0,1,\ldots,n-1$. The resulting $2^n$ group elements are distinct and have word length at most $3n$ with respect to any finite generating set containing $h$ and $t$. Hence the growth function is bounded below exponentially, and $H\wr\mathbb Z$ has exponential growth.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Write an element of $H\wr\mathbb Z$ as $(f,t^n)$. If it is central, commuting with $t$ makes the finitely supported lamp configuration $f$ invariant under translation. The only such configuration on the infinite set $\mathbb Z$ is the identity, so $f=1$. If $n\ne0$, then $t^n$ moves a nonidentity lamp at position zero to position $n$ and does not commute with it. Therefore $n=0$, and

$$
\boxed{Z(H\wr\mathbb Z)=1.}
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
