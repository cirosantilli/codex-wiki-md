# Paper 111

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20111.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III%20Paper%20111.pdf)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [root system](../../../semisimple-lie-algebra.md#root-system) in the real [inner product](../../../linear-algebra.md#inner-product) space $V$ is a finite spanning set $\Phi\subset V\setminus\{0\}$ such that

$$
\Phi\cap\mathbb R\alpha=\{\alpha,-\alpha\}
\quad\text{and}\quad
s_\alpha(\Phi)=\Phi
\qquad(\alpha\in\Phi),
$$

where the [orthogonal reflection](../../../linear-algebra.md#reflection-in-a-hyperplane)

$$
s_\alpha(v)=v-2\frac{(v,\alpha)}{(\alpha,\alpha)}\alpha.
$$

For a crystallographic root system one additionally requires $2(\beta,\alpha)/(\alpha,\alpha)\in\mathbb Z$; that condition is not needed for general finite reflection groups.

A [fundamental system of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) is a basis $\Delta\subset\Phi$ such that every root has either all nonnegative or all nonpositive coordinates in this basis. Its associated [positive system of a root system](../../../semisimple-lie-algebra.md#positive-system-of-a-root-system) is

$$
\Pi=\Phi\cap\operatorname{span}_{\mathbb R_{\geq0}}\Delta,
$$

and $\Phi=\Pi\sqcup(-\Pi)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [reflection group of a root system](../../../semisimple-lie-algebra.md#reflection-group-of-a-root-system) is

$$
W(\Phi)=\langle s_\alpha:\alpha\in\Phi\rangle\leq O(V).
$$

Every generating reflection permutes $\Phi$, so every $w\in W(\Phi)$ does too. If $\Delta$ is fundamental, then $w\Delta$ is a basis contained in $\Phi$. Writing

$$
\beta=\sum_{\alpha\in\Delta}c_\alpha\alpha
$$

shows that

$$
w\beta=\sum_{\alpha\in\Delta}c_\alpha w\alpha;
$$

the coefficients are unchanged and therefore still have one sign. Thus $w\Delta$ is another fundamental system, and $W(\Phi)$ acts on the set of all fundamental systems.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the [positive-root criterion for Coxeter length](../../../semisimple-lie-algebra.md#positive-root-criterion-for-coxeter-length): for a simple root $\alpha\in\Delta$,

$$
\ell(ws_\alpha)>\ell(w)
\quad\Longleftrightarrow\quad
w\alpha\in\Pi.
$$

The hypothesis $w\Delta\subseteq\Pi$ therefore says that every simple generator is a right ascent of $w$. If $w\ne1$, a [reduced expression in a Coxeter group](../../../lie-theory.md#reduced-expression-in-a-coxeter-group) for $w$ has a final simple generator $s_\alpha$, and deleting it gives

$$
\ell(ws_\alpha)=\ell(w)-1,
$$

a contradiction. Hence $w=1$.

If $w$ stabilizes $\Delta$ setwise, then $w\Delta=\Delta\subseteq\Pi$, so the result just proved gives $w=1$. Thus the stabilizer of every fundamental system is trivial.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

If a finitely generated [Coxeter group](../../../lie-theory.md#coxeter-group) $W$ is finite, its integer-valued [Coxeter length](../../../semisimple-lie-algebra.md#coxeter-length) has a maximum. Conversely, if some $w_0$ has globally maximal length $N$, every group element has a word of length at most $N$. There are only finitely many words of bounded length in the finite set of simple generators, so $W$ is finite.

Realize the finite group as the [reflection group of a root system](../../../semisimple-lie-algebra.md#reflection-group-of-a-root-system) with fundamental system $\Delta$ and positive system $\Pi$. Maximality and the fact that multiplication by a simple generator changes Coxeter length by one give

$$
\ell(w_0s_\alpha)=\ell(w_0)-1
\qquad(\alpha\in\Delta).
$$

The [positive-root criterion for Coxeter length](../../../semisimple-lie-algebra.md#positive-root-criterion-for-coxeter-length) therefore gives $w_0\Delta\subseteq-\Pi$. Since $w_0\Delta$ is itself fundamental, it must be the simple system $-\Delta$ of the positive system $-\Pi$.

If $v_0$ is another maximal-length element, the same argument gives $v_0\Delta=-\Delta=w_0\Delta$. Hence $v_0^{-1}w_0$ stabilizes $\Delta$, and part c gives $v_0^{-1}w_0=1$. The [longest element of a finite Coxeter group](../../../lie-theory.md#longest-element-of-a-coxeter-group) is therefore unique.

## 2

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/1">1</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/1/solution">Solution</h5>

↑ **Parent:** [1](#2/a/1)

Let $\phi=2\cos(\pi/5)=(1+\sqrt5)/2$. In the vertex order along the displayed $3$-$5$-$3$ path, the [Coxeter Gram matrix](../../../lie-theory.md#coxeter-gram-matrix) has diagonal entries $2$ and successive off-diagonal entries $-1,-\phi,-1$. Its leading principal determinants satisfy

$$
D_1=2,qquad D_2=3,qquad D_3=6-2\phi^2=4-2\phi,qquad D_4=2D_3-D_2=5-4\phi<0.
$$

The last determinant is nonzero, so the form is nondegenerate. Its negative determinant rules out positive semidefiniteness and hence also positive definiteness. Thus the answers are respectively no, no, and yes.

<h4 id="2/a/2">2</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/2/solution">Solution</h5>

↑ **Parent:** [2](#2/a/2)

The displayed simply-laced tree has arms of lengths $2$, $1$, and $3$ from its trivalent vertex, so it is the finite [type $E_7$ Coxeter graph](../../../lie-theory.md#e7-coxeter-group). Its Gram matrix is the $E_7$ Cartan matrix, which has positive leading principal minors in a leaf-removal ordering and determinant $2$. By [Sylvester's criterion](../../../linear-algebra.md#sylvester-s-criterion) it is positive definite. It is therefore positive semidefinite and nondegenerate as well: the three answers are yes, yes, and yes.

<h4 id="2/a/3">3</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/3/solution">Solution</h5>

↑ **Parent:** [3](#2/a/3)

For the four-cycle, the quadratic form is

$$
q(x)=\sum_{j=1}^4(x_j-x_{j+1})^2,
\qquad x_5=x_1.
$$

It is nonnegative, but it vanishes on the nonzero vector $(1,1,1,1)$. Equivalently, the Gram eigenvalues are $0,2,2,4$. The form is positive semidefinite, not positive definite, and degenerate: the three answers are no, yes, and no. This is the affine Coxeter graph $\widetilde A_3$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [exchange condition for a Coxeter group](../../../lie-theory.md#exchange-condition-for-a-coxeter-group) says that if $w=s_1\cdots s_n$ is reduced and $s$ is simple with $\ell(ws)<\ell(w)$, then

$$
ws=s_1\cdots\widehat{s_j}\cdots s_n
$$

for some $j$. The [Matsumoto theorem](../../../lie-theory.md#matsumoto-theorem) says that any two reduced expressions for the same element are connected by [braid moves](../../../lie-theory.md#braid-relation-in-a-coxeter-group). Together they imply the [Tits word reduction theorem](../../../lie-theory.md#tits-word-reduction-theorem): a nonreduced word can be transformed by braid moves until two equal adjacent generators can be cancelled.

For the displayed four-armed graph, call the central generator $s$ and the leaves $a,b,c,d$. Different leaves commute, while each leaf $t$ satisfies $sts=tst$. Consider the word

$$
u_N=(s\,a\,b\,s\,c\,d)^N.
$$

Between successive occurrences of $s$, the intervening leaf sets alternate between $\{a,b\}$ and $\{c,d\}$. Commuting the two leaves in one block never puts the same leaf on both sides of an $s$, so no length-three braid $tst\leftrightarrow sts$ is ever available. The only possible braid moves are those leaf commutations, and they cannot create adjacent equal letters. Tits reduction therefore shows that $u_N$ is reduced. Since $\ell(u_N)=6N$ is unbounded, the group is infinite.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the same graph, let $e_0$ correspond to the central vertex and $e_1,\ldots,e_4$ to the leaves. The associated simply-laced [Coxeter Gram matrix](../../../lie-theory.md#coxeter-gram-matrix) has

$$
(e_i,e_i)=2,qquad(e_0,e_j)=-1,qquad(e_i,e_j)=0
$$

for distinct leaves. The nonzero vector

$$
\delta=2e_0+e_1+e_2+e_3+e_4
$$

satisfies $(\delta,e_i)=0$ for every basis vector. Thus the form is degenerate; in fact it is positive semidefinite with one-dimensional radical, as expected for the affine graph $\widetilde D_4$.

The geometric form of a finite Coxeter group is positive definite. Since this form is degenerate, the group cannot be finite.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the [finite-dimensional vector-space topology](../../../topological-vector-space.md#finite-dimensional-vector-space-topology) on $V^*$: relative to the dual basis, it is the ordinary Euclidean topology on $\mathbb R^{|I|}$. Each coordinate map $f\mapsto f(e_i)$ is continuous, so

$$
H_i=\{f:f(e_i)=0\}
$$

is closed, while $A_i$, $A_i^-$, and the finite intersection $C=\bigcap_iA_i$ are open. Their closures are

$$
\overline{A_i}=\{f:f(e_i)\geq0\},
\qquad
\overline{A_i^-}=\{f:f(e_i)\leq0\},
\qquad
\overline C=D=\{f:f(e_i)\geq0\text{ for all }i\}.
$$

Every $\sigma^*(w)$ is an invertible linear map with inverse $\sigma^*(w^{-1})$. Linear maps between finite-dimensional topological vector spaces are continuous, so both it and its inverse are continuous. Hence every $\sigma^*(w)$ is a [homeomorphism](../../../topology.md#homeomorphism).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $f\in C$, duality gives

$$
(\sigma^*(w)f)(e_i)=f(\sigma(w^{-1})e_i).
$$

The [positive-root criterion for Coxeter length](../../../semisimple-lie-algebra.md#positive-root-criterion-for-coxeter-length) says

$$
\ell(x_iw)>\ell(w)
\quad\Longleftrightarrow\quad
\sigma(w^{-1})e_i
$$

is a positive root. Its basis coefficients are nonnegative and not all zero, so $f(\sigma(w^{-1})e_i)>0$ and $\sigma^*(w)(C)\subseteq A_i$. If the length decreases, that root is negative and the same calculation gives $\sigma^*(w)(C)\subseteq A_i^-$.

If $\sigma^*(w)$ is the identity and $w\ne1$, choose a left descent $x_i$ from the first letter of a reduced expression for $w$. The preceding result gives

$$
C=\sigma^*(w)(C)\subseteq A_i^-,
$$

although $C\subseteq A_i$. The two open half-spaces are disjoint, a contradiction. Thus the [Dual geometric representation of a Coxeter group](../../../lie-theory.md#dual-geometric-representation-of-a-coxeter-group) is faithful.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Suppose $\sigma^*(w)(C)$ meets $\sigma^*(v)(C)$. Applying the homeomorphism $\sigma^*(v^{-1})$ shows that $C$ meets $\sigma^*(v^{-1}w)(C)$. If $v^{-1}w\ne1$, choose one of its left descents. Part b places its image of $C$ in the corresponding negative half-space, while $C$ lies in the positive half-space. This is impossible, so $v=w$. The union

$$
\mathcal C=\bigsqcup_{w\in W}\sigma^*(w)(C)
$$

is disjoint.

When $W$ is finite, the closures $\sigma^*(w)(D)$ are the simplicial chambers cut out by the reflecting hyperplanes. Intersecting them with a sphere centred at the origin gives simplices. A face of type $J\subseteq I$ has stabilizer the [standard parabolic subgroup](../../../lie-theory.md#standard-parabolic-subgroup) $W_J$, so its translates are indexed by cosets $wW_J$, with reverse inclusion of cosets encoding incidence. This is precisely the [Coxeter complex](../../../lie-theory.md#coxeter-complex) of $(W,I)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

If $W$ is finite, its finitely many reflecting hyperplanes divide $V^*$ into chambers, and the closures of these chambers are exactly the translates $\sigma^*(w)(D)$. Hence the [Tits cone](../../../lie-theory.md#tits-cone)

$$
U=\bigcup_{w\in W}\sigma^*(w)(D)
$$

equals $V^*$.

Conversely, suppose $W$ is infinite and choose $f\in-C$, so $f(e_i)<0$ for every $i$. If $f\in U$, then $f\in\sigma^*(w)(D)$ for some $w$, and therefore

$$
f(\sigma(w)e_i)=(\sigma^*(w^{-1})f)(e_i)\geq0
$$

for every $i$. Since $f$ is strictly negative on every positive root and strictly positive on every negative root, each $\sigma(w)e_i$ must be negative. The length criterion gives

$$
\ell(wx_i)<\ell(w)
$$

for every $i$. This contradicts the stated fact that in an infinite Coxeter group the length of every element can be increased by multiplication on the right by some simple generator. Thus $-C$ is not contained in $U$, and $U\ne V^*$.

## 4

↑ **Parent:** [Paper 111](paper-111.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Reversing a word for $w$ gives a word of the same length for $w^{-1}$ because every generator is an [involution](../../../group-theory.md#involution). Applying the same argument to $w^{-1}$ proves

$$
\ell_S(w^{-1})=\ell_S(w).
$$

A shortest word for $w$ followed by $s_i$ gives $\ell_S(ws_i)\leq\ell_S(w)+1$. Conversely, $w=(ws_i)s_i$ gives $\ell_S(w)\leq\ell_S(ws_i)+1$. Hence

$$
\boxed{\ell_S(ws_i)\in\{\ell_S(w)-1,\ell_S(w),\ell_S(w)+1\}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

We prove the assertion by induction on $n$. Write $w=av$, where $a=s_{i_1}$ and $v=s_{i_2}\cdots s_{i_n}$; both displayed words are reduced. The first clause of the [folding condition](../../../lie-theory.md#folding-condition) and part a imply that $\ell(vs)$ is either $n-2$ or $n$.

If $\ell(vs)=n-2$, the induction hypothesis deletes one unique letter from the reduced word for $v$. Prefixing $a$ gives the required deletion from $w$. If another deletion were possible, induction rules out another internal position, while deletion of $a$ would give $ws=v$ and hence $vs=av$, contradicting the lengths $n-2$ and $n$.

If $\ell(vs)=n$, both $av$ and $vs$ increase the length of $v$. Since $\ell(avs)=\ell(ws)=n-1$, the other alternative in the folding condition must hold:

$$
v=avs.
$$

Thus $ws=avs=v$, which deletes the first letter. An additional internal deletion would give $v=a v'$ for a word $v'$ of length $n-2$; multiplying by $a$ would make the length-$n$ element $av=w$ equal to $v'$, impossible. The deletion position is therefore unique in every case.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

If $m_{ij}<\infty$, the [braid relation in a Coxeter group](../../../lie-theory.md#braid-relation-in-a-coxeter-group) is

$$
\underbrace{s_is_js_i\cdots}_{m_{ij}\text{ factors}}
=
\underbrace{s_js_is_j\cdots}_{m_{ij}\text{ factors}}.
$$

For $m_{ij}=2$ this is commutation; no relation is imposed when $m_{ij}=\infty$. Two reduced expressions are braid equivalent when one can be transformed into the other by finitely many replacements of one side of such a relation by the other.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

First suppose $(W,S)$ is a [Coxeter system](../../../lie-theory.md#coxeter-system). The usual exchange condition implies that multiplication by a simple generator changes length by exactly one. Let $w=t_1\cdots t_n$ be reduced and suppose both $s_iw$ and $ws_j$ have length $n+1$. The length of $s_iws_j$ is therefore either $n+2$ or $n$. In the latter case, apply exchange to the reduced word $s_i t_1\cdots t_n$ followed by $s_j$. If exchange deleted one of the $t_k$, multiplying the resulting equality on the left by $s_i$ would express the length-$n+1$ element $ws_j$ using only $n-1$ generators. Hence exchange must delete the initial $s_i$, giving $s_iws_j=w$. This is exactly the folding condition.

Conversely, suppose the folding condition holds, and let $W_M$ be the abstract Coxeter group with generators $S$ and matrix $(m_{ij})$. The defining relations hold in $W$, so there is a surjective homomorphism

$$
\pi:W_M\longrightarrow W.
$$

It remains to prove injectivity. Take any word in the kernel. If its image word in $W$ is not reduced, choose its shortest nonreduced prefix $ut$, where $u$ is reduced and $t$ is its last generator. Part b gives $ut=v$, where $v$ is obtained by deleting one letter from $u$. Hence $u=vt$, and $u$ and $vt$ are two reduced expressions for the same element. By the assumed braid-equivalence theorem they are related by braid moves. Those moves are defining relations in $W_M$, after which the end of the prefix becomes $vtt$ and $t^2=1$ shortens the original word by two.

Repeating this process turns the kernel word, using only Coxeter relations, into a word that is reduced in $W$. Since its image is the identity, that reduced word is empty. The original word is therefore already the identity in $W_M$, so $\ker\pi=1$. Hence $W\cong W_M$ is the Coxeter group with generators $S$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
