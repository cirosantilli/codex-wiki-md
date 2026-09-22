# Paper 101

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_101.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_101.pdf)

**Table of contents**

- [1](#1)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [ideal of definition](../../../algebra.md#ideal-of-definition) of a [Noetherian local ring](../../../algebra.md#noetherian-local-ring) $(A,\mathfrak m)$ is an $\mathfrak m$-primary ideal $I$; equivalently, $\sqrt I=\mathfrak m$, or some power $\mathfrak m^r$ is contained in $I$.

If $M$ is a finitely generated module of dimension $d$, the [Hilbert–Samuel function](../../../commutative-algebra.md#hilbert-samuel-function)

$$
\chi(M,I;n)=\ell(M/I^nM)
$$

agrees for all sufficiently large $n$ with a polynomial of degree $d$. Its leading term is

$$
\frac{e_I(M)}{d!}n^d,
$$

where $e_I(M)$ is the [Hilbert–Samuel multiplicity](../../../commutative-algebra.md#hilbert-samuel-multiplicity).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Assume first that $f\ne0$ and let

$$
d=\operatorname{ord}_{(x,y)}f
$$

be the least total degree of a nonzero homogeneous part of $f$. The [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) is

$$
\operatorname{gr}_{\mathfrak m}A
\simeq k[x,y]/(f_d),
$$

where $f_d$ is the initial homogeneous form. Multiplication by the nonzero polynomial $f_d$ is injective in $k[x,y]$, so the degree-$j$ component has dimension

$$
\dim_k(\operatorname{gr}_{\mathfrak m}A)_j
=\begin{cases}j+1,&j<d,\\d,&j\geq d.\end{cases}
$$

Summing the components of degrees below $n$ gives

$$
\boxed{
\chi(A,\mathfrak m;n)=
\begin{cases}
n(n+1)/2,&n\leq d,\\
dn-d(d-1)/2,&n\geq d.
\end{cases}}
$$

Thus the [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial) is

$$
\boxed{P(n)=dn-\frac{d(d-1)}2.}
$$

Its leading coefficient is the order of vanishing, or multiplicity, of the plane curve $f=0$ at the origin. If $f=0$, no relation is imposed and $\chi=n(n+1)/2$ for every $n$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A monomial of weighted degree $n$ is $x^{n-2j}y^j$ with $0\leq j\leq\lfloor n/2\rfloor$. Therefore

$$
\boxed{F_S(n)=\dim_kS_n=\left\lfloor\frac n2\right\rfloor+1.}
$$

This is a [quasipolynomial](../../../commutative-algebra.md#quasipolynomial) of period two, not eventually one polynomial: it equals $n/2+1$ for even $n$ and $(n+1)/2$ for odd $n$. The usual eventual-polynomial theorem for a graded algebra assumes a [standard graded algebra](../../../commutative-algebra.md#standard-graded-algebra), generated in degree one. Here the generator $y$ has degree two, so there is no contradiction.

## 2

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The ring of [p-adic integers](../../../number-theory.md#p-adic-integer) is the inverse limit

$$
\boxed{\mathbb Z_p=\varprojlim_n\mathbb Z/p^n\mathbb Z.}
$$

Equivalently, each element has a unique convergent expansion $\sum_{j\geq0}b_jp^j$ with digits $0\leq b_j<p$. It is a complete discrete valuation ring with maximal ideal $(p)$ and residue field $\mathbb F_p$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Addition preserves the condition because

$$
\operatorname{ord}(a_n+b_n)\geq
\min\{\operatorname{ord}(a_n),\operatorname{ord}(b_n)\}.
$$

For multiplication, write $c_n=\sum_{i+j=n}a_ib_j$. Given $q$, choose $N$ so that $a_i,b_i\in p^q\mathbb Z_p$ for $i\geq N$. If $n\geq2N$, every pair $i+j=n$ has $i\geq N$ or $j\geq N$, so every summand lies in $p^q\mathbb Z_p$. Hence $\operatorname{ord}(c_n)\to\infty$, proving that $\mathbb Z_p\langle T\rangle$ is a subring of the [formal power series ring](../../../commutative-algebra.md#formal-power-series) $\mathbb Z_p[[T]]$.

The $(p)$-adic completion is

$$
\widehat{\mathbb Z[T]}
=\varprojlim_q\mathbb Z[T]/p^q\mathbb Z[T]
=\varprojlim_q(\mathbb Z/p^q\mathbb Z)[T].
$$

A compatible system of polynomials determines coefficients $a_n\in\mathbb Z_p$. For each $q$, its reduction has finite degree, so all but finitely many $a_n$ lie in $p^q\mathbb Z_p$. This is exactly $\operatorname{ord}(a_n)\to\infty$. Conversely, every such restricted series reduces modulo $p^q$ to a polynomial and hence defines a compatible system. Therefore

$$
\boxed{\widehat{\mathbb Z[T]}^{(p)}\simeq\mathbb Z_p\langle T\rangle.}
$$

## 3

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An element lies in $\mathfrak p^*$ exactly when all its homogeneous components lie in $\mathfrak p$. Suppose $ab\in\mathfrak p^*$ but $a,b\notin\mathfrak p^*$. Choose the least-degree components $a_i\notin\mathfrak p$ and $b_j\notin\mathfrak p$. In the degree $i+j$ component of $ab$, every term other than $a_ib_j$ contains a lower component of $a$ or $b$ and hence lies in $\mathfrak p$. Since the whole component lies in $\mathfrak p$, it follows that $a_ib_j\in\mathfrak p$, contradicting primality. Thus

$$
\boxed{\mathfrak p^*\text{ is prime}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

First, $\sqrt{\mathfrak q^*}=\mathfrak p$. Indeed, each homogeneous element of $\mathfrak p=\sqrt{\mathfrak q}$ has a power in $\mathfrak q$, and that power is homogeneous and hence lies in $\mathfrak q^*$; finite homogeneous generators of the Noetherian ideal $\mathfrak p$ give the assertion for every element.

Now suppose $ab\in\mathfrak q^*$ and $a\notin\mathfrak p$. Choose the least homogeneous component $a_i\notin\mathfrak p$. If $b\notin\mathfrak q^*$, choose the least component $b_j\notin\mathfrak q$. The degree $i+j$ component of $ab$ differs from $a_ib_j$ by terms in $\mathfrak q$. Since it lies in $\mathfrak q$, we get $a_ib_j\in\mathfrak q$. The $\mathfrak p$-primary property and $a_i\notin\mathfrak p$ imply $b_j\in\mathfrak q$, a contradiction. Hence $b\in\mathfrak q^*$, proving that

$$
\boxed{\mathfrak q^*\text{ is }\mathfrak p\text{-primary}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Pass to the graded domain $R=S/\mathfrak p^*$ and let $\overline{\mathfrak p}=\mathfrak p/\mathfrak p^*$. This is a nonzero prime containing no nonzero homogeneous element. Localize at the multiplicative set $U$ of all nonzero homogeneous elements. Every nonzero homogeneous element of $U^{-1}R$ is a unit; its nonzero graded pieces are one-dimensional over the degree-zero field, so after reindexing degrees this localization is a Laurent polynomial ring $K[t,t^{-1}]$. The extended prime $U^{-1}\overline{\mathfrak p}$ is therefore a nonzero prime of height one.

Any prime strictly between $0$ and $\overline{\mathfrak p}$ would remain a nonzero prime strictly below it after localization, impossible in $K[t,t^{-1}]$. Contracting back proves that no prime lies strictly between $\mathfrak p^*$ and $\mathfrak p$. The graded height theorem, equivalently the same localization argument applied to saturated chains, then gives

$$
\boxed{\operatorname{ht}(\mathfrak p)
=\operatorname{ht}(\mathfrak p^*)+1.}
$$

## 4

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Choose a finite presentation $F_1\to F_0\to M\to0$ with $F_0,F_1$ finite free. Applying $\operatorname{Hom}_A(-,A)$ gives

$$
0\longrightarrow M^*\longrightarrow F_0^*
\longrightarrow F_1^*.
$$

Let $N=F_0^*$ and let $P$ be the image in $F_1^*$. Then

$$
\boxed{0\longrightarrow M^*\longrightarrow N
\longrightarrow P\longrightarrow0}
$$

is exact, $N$ is finite free, and $P$ is torsion-free because it is a submodule of the free module $F_1^*$ over the domain $A$.

The [reflexive-module second-syzygy criterion](../../../module-theory.md#reflexive-module-second-syzygy-criterion) says that the kernel of a map from a finite free module to a torsion-free module over a Noetherian domain is reflexive. Applying it to this sequence shows that $M^*$ is reflexive. Concretely, after localizing at the fraction field, every functional on $(M^*)^*$ represented generically by an element of $N$ has no denominator: torsion-freeness of $P$ forces its image to vanish already over $A$. Thus the natural evaluation map $M^*\to M^{***}$ is an isomorphism.

## 5

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Put $g=y^2-zw$. Every generator of $I$ is divisible by $x^2$ and belongs to $(y,z)^2$, while the displayed decomposition in the next part will show that

$$
\sqrt I=(x)\cap(y,z).
$$

Its two minimal primes, and hence its isolated associated primes, are

$$
\boxed{\mathfrak p_1=(x),
\qquad \mathfrak p_2=(y,z).}
$$

The corresponding isolated primary components are

$$
\boxed{\mathfrak q_1=(x^2),
\qquad \mathfrak q_2=(y,z)^2=(y^2,yz,z^2).}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Consider

$$
\mathfrak q_3=(x^3,y^2-zw).
$$

It is $(x,y^2-zw)$-primary. A direct ideal-intersection calculation gives

$$
\begin{aligned}
\mathfrak q_1\cap\mathfrak q_2\cap\mathfrak q_3
&=x^2\big[(y,z)^2\cap(x,g)\big]\\
&=x^2\big[x(y,z)^2+g(y,z)\big]\\
&=(x^3y^2,x^3yz,x^3z^2,x^2y(y^2-zw),x^2z(y^2-zw))\\
&=I.
\end{aligned}
$$

This decomposition is irredundant and its radicals are

$$
(x),\qquad(y,z),\qquad(x,y^2-zw).
$$

Therefore

$$
\boxed{\operatorname{Ass}(k[x,y,z,w]/I)
=\{(x),(y,z),(x,y^2-zw)\}.}
$$

In particular, $\mathfrak p_3=(x,y^2-zw)$ is the embedded associated prime and the decomposition also confirms $\sqrt I=(x)\cap(y,z)$.

## 6

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Restriction of scalars makes every $S^{-1}A$-module an $A$-module, and multiplication by $s\in S$ is invertible with inverse multiplication by $1/s$.

Conversely, suppose each multiplication map $s_M:m\mapsto sm$ is an automorphism of the $A$-module $M$. Define

$$
\frac as\cdot m=a\,s_M^{-1}(m).
$$

The universal property of localization shows that this is well-defined and gives the unique $S^{-1}A$-module structure extending the $A$-action. These constructions are inverse.

Under this structure the natural map $M\to S^{-1}M$ has inverse

$$
\boxed{\frac ms\longmapsto s_M^{-1}(m),}
$$

so it is an isomorphism.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Localization of the inclusion $N\hookrightarrow M$ gives an injection $S^{-1}N\hookrightarrow S^{-1}M$, whose image lies in $N'$. Conversely, take $m/s\in N'$. Since $s/1$ is a unit and $N'$ is an $S^{-1}A$-submodule,

$$
\frac m1=\frac s1\frac ms\in N'.
$$

By the definition of the inverse image, $m\in N$, and hence $m/s$ lies in the image of $S^{-1}N$. Therefore

$$
\boxed{N'\simeq S^{-1}N.}
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
