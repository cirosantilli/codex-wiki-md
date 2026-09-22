# Paper 145

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20145.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20145.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 145](paper-145.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For edge weights $w_{ij}$, form the out-Laplacian

$$
L_{ij}=\begin{cases}
\sum_{k\ne i}w_{ik},&i=j,\\
-w_{ij},&i\ne j.
\end{cases}
$$

The directed [matrix-tree theorem](../../../combinatorics.md#kirchhoff-s-theorem) states that the cofactor $\det L^{(r)}$, obtained by deleting row and column $r$, equals the sum of $\prod_{e\in T}w_e$ over directed spanning trees oriented towards $r$.

Expand the determinant by permutations, and in each diagonal entry expand the sum of outgoing edge weights. A term chooses one outgoing edge at every vertex other than $r$. If the resulting functional digraph contains a directed cycle, sign-reversing inclusion-exclusion over its cycles cancels the term. The surviving choices are precisely the acyclic ones; every vertex then reaches $r$, so they are rooted directed spanning trees, each with positive sign and its product weight. This proves the theorem.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Give every edge weight one and delete the row and column for $v_n$ from the out-Laplacian. Expanding the resulting banded determinant along its last available row gives

$$
a_n=a_{n-1}+2a_{n-2},
\qquad a_2=1,\quad a_3=3.
$$

The characteristic roots are $2$ and $-1$, and the initial values give

$$
a_n=\frac{2^n-(-1)^n}{3}.
$$

By the directed [matrix-tree theorem](../../../combinatorics.md#kirchhoff-s-theorem), this determinant is exactly the number of directed spanning trees rooted towards $v_n$.

## 2

↑ **Parent:** [Paper 145](paper-145.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Stirling number of the second kind](../../../combinatorics.md#stirling-numbers-of-the-second-kind) $\left\{\begin{smallmatrix}n\\k\end{smallmatrix}\right\}$ counts partitions of an $n$-element set into $k$ nonempty unlabeled blocks. Distinguishing the block containing the last element gives

$$
\left\{\begin{matrix}n\\k\end{matrix}\right\}
=k\left\{\begin{matrix}n-1\\k\end{matrix}\right\}
+\left\{\begin{matrix}n-1\\k-1\end{matrix}\right\}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a positive integer $x$, count functions $[n]\to[x]$ by the number $k$ of nonempty fibres. Their fibres form a $k$-block partition in $\left\{\begin{smallmatrix}n\\k\end{smallmatrix}\right\}$ ways, and the blocks receive distinct images in $x^{\underline k}$ ways. Hence

$$
x^n=\sum_{k=1}^n\left\{\begin{matrix}n\\k\end{matrix}\right\}x^{\underline k}.
$$

Both sides are polynomials of degree $n$ agreeing at every positive integer, so this is a polynomial identity.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Partitions of the vertices into independent blocks are the unlabeled colour-class partitions counted by the [Graphical Stirling number](../../../combinatorics.md#graphical-stirling-number). Therefore

$$
\chi_{P_n}(x)=\sum_k\left\{\begin{matrix}n\\k\end{matrix}\right\}_{P_n}x^{\underline k}.
$$

Since $\chi_{P_n}(x)=x(x-1)^{n-1}$, the ordinary Stirling identity applied to $x-1$ gives

$$
x(x-1)^{n-1}
=\sum_k\left\{\begin{matrix}n-1\\k-1\end{matrix}\right\}x^{\underline k}.
$$

Uniqueness in the falling-factorial basis proves the claim.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The sum is the chromatic polynomial of the path, so

$$
\sum_{k=1}^n
\left\{\begin{matrix}n\\k\end{matrix}\right\}_{P_n}
x^{\underline k}
=x(x-1)^{n-1}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

In an independent-block partition of $P_n$, either $v_1,v_n$ lie in different blocks, giving a partition valid for $C_n$, or they lie in the same block. Contracting those endpoints in the second case gives an independent-block partition of $C_{n-1}$. This bijection proves the recurrence. Multiplying by $x^{\underline k}$ and summing gives

$$
\chi_{P_n}(x)=\chi_{C_n}(x)+\chi_{C_{n-1}}(x).
$$

Using $\chi_{P_n}=x(x-1)^{n-1}$ and induction from $C_2=P_2$ yields

$$
\boxed{\chi_{C_n}(x)=(x-1)^n+(-1)^n(x-1).}
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

A proper colouring using exactly $k$ colours first partitions the vertices into $k$ nonempty independent colour classes and then injectively assigns $k$ of the $x$ named colours to those classes. These choices number

$$
\left\{\begin{matrix}n\\k\end{matrix}\right\}_Gx^{\underline k}.
$$

Summing over $k$ counts every proper colouring exactly once; the expression is the [chromatic polynomial](../../../graph-theory.md#chromatic-polynomial) $\chi_G(x)$.

## 3

↑ **Parent:** [Paper 145](paper-145.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A nonempty [Dyck path](../../../combinatorics.md#dyck-path) decomposes uniquely as an up-step, a Dyck path, a down-step, and another Dyck path. Marking each matched outer pair by $x$ gives

$$
C(x)=1+xC(x)^2.
$$

The solution with constant term one is

$$
\boxed{C(x)=\frac{1-\sqrt{1-4x}}{2x}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Deleting the first up-step and last down-step of a strictly positive walk of semilength $n$ and lowering the remainder by one gives a Dyck path of semilength $n-1$, bijectively. Hence $D_n=C_{n-1}$ and

$$
\boxed{D(x)=\sum_{n\geq1}D_nx^n=xC(x).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A strictly negative primitive excursion of semilength $n$ has all $2n$ steps negative, so weight $\sqrt t^{\,2n}=t^n$. Reflection in the axis identifies it with a strictly positive excursion, giving

$$
E(x)=\sum_{n\geq1}D_n(tx)^n=D(tx).
$$

Every bridge has a unique decomposition at successive returns to the axis into positive or negative primitive excursions. The sequence construction therefore has generating function

$$
\frac1{1-D(x)-E(x)}.
$$

Its exponent of $t$ is half the number of negative steps, proving the asserted interpretation of $f(t,n)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Since $D(x)=xC(x)=(1-\sqrt{1-4x})/2$,

$$
\frac1{1-D(x)-D(tx)}
=\frac2{\sqrt{1-4x}+\sqrt{1-4tx}}.
$$

Rationalizing and using the Catalan generating function gives

$$
\frac2{\sqrt{1-4x}+\sqrt{1-4tx}}
=\sum_{n\geq0}C_nx^n(1+t+\cdots+t^n).
$$

**Thus the coefficient of every $t^k$, $0\leq k\leq n$, is $C_n$. The number of bridges with exactly $2k$ negative steps is consequently independent of $k$.**

## 4

↑ **Parent:** [Paper 145](paper-145.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $v_i\in\mathbb F_2^n$ be the incidence vector of $S_i$. Then

$$
v_i\cdot v_i=|S_i|\equiv1\pmod2,
\qquad
v_i\cdot v_j=|S_i\cap S_j|\equiv0\pmod2
$$

for $i\ne j$. If $\sum_i c_iv_i=0$, taking the dot product with $v_j$ gives $c_j=0$. The vectors are linearly independent, so $m\leq n$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The required prime-power form of the [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) is: if $A_1,\ldots,A_m\subseteq[n]$, no $|A_i|$ is divisible by $p^r$, and every intersection of $k$ distinct members has size divisible by $p^r$, then

$$
m\leq(k-1)(n+1).
$$

It follows by associating to each $A_i$ its incidence vector augmented by a constant coordinate and applying the Frankl-Wilson polynomial independence lemma to the $(k-1)$ layers of multilinear intersection polynomials. The hypotheses make the diagonal evaluations nonzero modulo $p^r$ and every $k$-fold off-diagonal evaluation zero; independence leaves at most $(k-1)(n+1)$ polynomials. Applying the theorem gives the desired bound.

When $r=1$, the argument works directly over $\mathbb F_p$ without the constant-coordinate lift and yields the stronger bound

$$
m\leq(k-1)n.
$$

**Therefore a family of size $(k-1)(n+1)$ does not exist.**

## 5

↑ **Parent:** [Paper 145](paper-145.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [Alon-Tarsi lemma](../../../combinatorics.md#alon-tarsi-lemma) says that if $\deg f\leq d_1+\cdots+d_n$ and $A_i$ consists of $d_i+1$ distinct field elements, then

$$
[x_1^{d_1}\cdots x_n^{d_n}]f
=\sum_{a_i\in A_i}
\frac{f(a_1,\ldots,a_n)}
{\prod_i\prod_{b\in A_i\setminus\{a_i\}}(a_i-b)}.
$$

This follows by applying univariate Lagrange interpolation successively in each variable.

If the displayed coefficient is nonzero, at least one summand has $f(a_1,\ldots,a_n)\ne0$. This is the coefficient form of the [Combinatorial Nullstellensatz](../../../combinatorics.md#combinatorial-nullstellensatz).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Write each hyperplane as $h_j(x)=0$, normalized so that $h_j(0)=1$, and put

$$
P(x)=\prod_{j=1}^m h_j(x).
$$

Then $P(0)=1$ and $P$ vanishes at every other point of $\mathbb F_q^n$. Reduce $P$ modulo $x_i^q-x_i$ in every variable. This preserves its function on $\mathbb F_q^n$, does not increase total degree, and gives the unique representative with each variable degree at most $q-1$.

The unique reduced polynomial for the delta function at zero is

$$
\prod_{i=1}^n(1-x_i^{q-1}),
$$

whose total degree is $(q-1)n$. Hence

$$
m=\deg P\geq(q-1)n.
$$

Uniqueness follows equally from the Alon-Tarsi lemma on the grids $A_i=\mathbb F_q$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
