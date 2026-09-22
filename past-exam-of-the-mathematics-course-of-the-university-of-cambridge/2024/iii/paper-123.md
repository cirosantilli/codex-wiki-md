# Paper 123

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_123.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_123.pdf)

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
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
  - [f](#3/f)
    - [Solution](#3/f/solution)
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
  - [e](#5/e)
    - [Solution](#5/e/solution)

## 1

↑ **Parent:** [Paper 123](paper-123.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [modulus of a number field](../../../algebraic-number-theory.md#modulus-of-a-number-field) is a formal product

$$
\mathfrak m=\mathfrak m_0\mathfrak m_\infty,
$$

where $\mathfrak m_0=\prod_{\mathfrak p}\mathfrak p^{n_\mathfrak p}$ is a nonzero integral ideal and $\mathfrak m_\infty$ is a product of distinct real embeddings of $K$. Only finitely many $n_\mathfrak p$ are nonzero; complex places do not occur.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $I_K(\mathfrak m)$ be the group of fractional ideals prime to $\mathfrak m_0$. Let $P_K(\mathfrak m)$ consist of principal ideals $(\alpha)$ with

$$
\alpha\equiv1\pmod{\mathfrak p^{n_\mathfrak p}}
$$

for every $\mathfrak p\mid\mathfrak m_0$ and $\sigma(\alpha)>0$ for every real place $\sigma\mid\mathfrak m_\infty$. The [ray class group](../../../algebraic-number-theory.md#ray-class-group) is

$$
\boxed{\operatorname{Cl}_{\mathfrak m}(K)
=I_K(\mathfrak m)/P_K(\mathfrak m).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let

$$
U_{\mathfrak m,1}
=\{u\in\mathcal O_K^\times:
u\equiv1\pmod{\mathfrak m_0},\
\sigma(u)>0\text{ for }\sigma\mid\mathfrak m_\infty\}.
$$

The [ray class number formula](../../../algebraic-number-theory.md#ray-class-number-formula) is

$$
\boxed{|\operatorname{Cl}_{\mathfrak m}(K)|
=h_K\frac{2^{|\mathfrak m_\infty|}
N\mathfrak m_0
\prod_{\mathfrak p\mid\mathfrak m_0}(1-N\mathfrak p^{-1})}
{[\mathcal O_K^\times:U_{\mathfrak m,1}]}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The quadratic field $K=\mathbb Q(\sqrt{-7})$ is the unique quadratic subfield of $\mathbb Q(\zeta_7)$. Its nontrivial character is the quadratic character

$$
\chi_7(a)=\left(\frac a7\right).
$$

Under the [Artin reciprocity map](../../../algebraic-number-theory.md#artin-reciprocity-law), Frobenius at an unramified prime $p$ restricts trivially to $K$ exactly when $\chi_7(p)=1$. The quadratic residues modulo $7$ are $1,2,4$, while $5$ is a nonresidue. Thus

$$
\chi_7(5)=-1,
$$

so the Artin symbol at $5$ is the nonidentity element of $\operatorname{Gal}(K/\mathbb Q)$. Therefore $5$ has residue degree two and is inert in $K$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Since $5$ is inert, $\mathfrak m=5\mathcal O_K$ is prime and

$$
N\mathfrak m=25,\qquad
|(\mathcal O_K/\mathfrak m)^\times|=24.
$$

The unit group is $\{\pm1\}$, and only $1$ is congruent to $1$ modulo $\mathfrak m$, so

$$
[\mathcal O_K^\times:U_{\mathfrak m,1}]=2.
$$

There are no real places and $h_K=1$. The [ray class number formula](../../../algebraic-number-theory.md#ray-class-number-formula) gives

$$
|\operatorname{Cl}_{\mathfrak m}(K)|=\frac{24}{2}=12.
$$

Hence the [ray class field](../../../algebraic-number-theory.md#ray-class-field) modulo $5\mathcal O_K$ has degree $\boxed{12}$ over $K$.

## 2

↑ **Parent:** [Paper 123](paper-123.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an unramified prime $\mathfrak p$ of $K$ and a prime $\mathfrak P$ of $L$ above it, the Frobenius automorphism is characterized by

$$
\operatorname{Frob}_{\mathfrak P/\mathfrak p}(x)
\equiv x^{N\mathfrak p}\pmod{\mathfrak P}.
$$

In an abelian extension it is independent of $\mathfrak P$. This element is the [Artin symbol](../../../algebraic-number-theory.md#artin-symbol)

$$
\boxed{\left(\frac{L/K}{\mathfrak p}\right).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Every ideal of $\mathbb Z$ prime to $8$ has a representative $n\mathbb Z$ with $n$ odd and positive. The [Artin reciprocity map](../../../algebraic-number-theory.md#artin-reciprocity-law) for $\mathbb Q(\zeta_8)/\mathbb Q$ is

$$
n\mathbb Z\longmapsto\sigma_n,\qquad
\sigma_n(\zeta_8)=\zeta_8^n.
$$

Its kernel consists exactly of positive principal ideals generated by numbers congruent to $1$ modulo $8$. Therefore

$$
I_{\mathbb Q}(8\infty)/P_{\mathbb Q}(8\infty)
\cong\operatorname{Gal}(\mathbb Q(\zeta_8)/\mathbb Q)
\cong(\mathbb Z/8\mathbb Z)^\times,
$$

and the four classes are

$$
\boxed{[\mathbb Z],[3\mathbb Z],[5\mathbb Z],[7\mathbb Z].}
$$

Complex conjugation sends $\zeta_8$ to $\zeta_8^{-1}=\zeta_8^7$, so it corresponds to $\boxed{7}$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Under the preceding quotient, $H/P_{\mathbb Q}(8\infty)$ is the subgroup

$$
\{1,7\}\leq(\mathbb Z/8\mathbb Z)^\times.
$$

It has order two in a group of order four. Hence $H$ contains $P_{\mathbb Q}(8\infty)$ and

$$
\boxed{[I_{\mathbb Q}(8\infty):H]=2.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The ideal-theoretic [existence theorem of global class field theory](../../../algebraic-number-theory.md#existence-theorem-of-global-class-field-theory) gives an inclusion-reversing correspondence between finite abelian extensions $L/K$ and congruence subgroups

$$
P_K(\mathfrak m)\subseteq H\subseteq I_K(\mathfrak m).
$$

The corresponding field satisfies

$$
\boxed{H=\ker\!\left(I_K(\mathfrak m)
\xrightarrow{\operatorname{Art}_{L/K}}
\operatorname{Gal}(L/K)\right),
\qquad
I_K(\mathfrak m)/H\cong\operatorname{Gal}(L/K).}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The subgroup $H/P_{\mathbb Q}(8\infty)=\{1,7\}$ corresponds inside $\mathbb Q(\zeta_8)$ to the fixed field of $\{1,c\}$, where $c$ is complex conjugation. This is the maximal real subfield

$$
\mathbb Q(\zeta_8+\zeta_8^{-1})
=\mathbb Q(\sqrt2).
$$

Thus the [existence theorem of global class field theory](../../../algebraic-number-theory.md#existence-theorem-of-global-class-field-theory) associates $H$ with $\boxed{\mathbb Q(\sqrt2)}$.

## 3

↑ **Parent:** [Paper 123](paper-123.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [Dirichlet character](../../../algebraic-number-theory.md#dirichlet-character) modulo $m$ is a homomorphism

$$
\chi:(\mathbb Z/m\mathbb Z)^\times\to\mathbb C^\times.
$$

Extend it periodically to $\mathbb Z$ by setting $\chi(n)=0$ when $(n,m)>1$. Its [Dirichlet L-function](../../../algebraic-number-theory.md#dirichlet-l-function) is

$$
\boxed{L(s,\chi)=\sum_{n\geq1}\frac{\chi(n)}{n^s}
=\prod_p(1-\chi(p)p^{-s})^{-1}
\qquad(\operatorname{Re}s>1).}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Dedekind zeta function](../../../algebraic-number-theory.md#dedekind-zeta-function) of $K$ is

$$
\boxed{\zeta_K(s)=
\sum_{0\neq\mathfrak a\subseteq\mathcal O_K}
N(\mathfrak a)^{-s}
=\prod_{\mathfrak p}
(1-N\mathfrak p^{-s})^{-1}}
$$

for $\operatorname{Re}s>1$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

By the [Kronecker–Weber theorem](../../../algebraic-number-theory.md#kronecker-weber-theorem), choose $m$ with

$$
K\subseteq\mathbb Q(\zeta_m).
$$

Restriction gives a quotient

$$
(\mathbb Z/m\mathbb Z)^\times
\twoheadrightarrow G=\operatorname{Gal}(K/\mathbb Q).
$$

Every character $\psi\in\widehat G$ inflates along this quotient and has an associated primitive Dirichlet character $\chi_\psi$, whose conductor may divide $m$. Comparing Euler factors, or applying the factorization of the Artin $L$-function of the regular representation, gives

$$
\boxed{\zeta_K(s)=
\prod_{\psi\in\widehat G}L(s,\chi_\psi).}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The group $(\mathbb Z/7\mathbb Z)^\times$ is cyclic of order six, generated by $3$. Put $\omega=e^{2\pi i/6}$. The six characters are

$$
\chi_j(3^r)=\omega^{jr},
\qquad 0\leq j\leq5,
$$

and vanish on multiples of $7$. Since

$$
(3^0,3^1,\ldots,3^5)\equiv(1,3,2,6,4,5)\pmod7,
$$

their values are explicitly

$$
\begin{array}{c|rrrrrr}
a&1&2&3&4&5&6\\ \hline
\chi_j(a)&1&\omega^{2j}&\omega^j&\omega^{4j}&\omega^{5j}&\omega^{3j}.
\end{array}
$$

Taking $j=0,\ldots,5$ lists all six characters.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The unique order-two character is $\chi_3$, the Legendre symbol

$$
\chi_3(a)=\left(\frac a7\right).
$$

It is $1$ on $1,2,4$, is $-1$ on $3,5,6$, and is zero on multiples of $7$. Since the unique quadratic subfield of $\mathbb Q(\zeta_7)$ is $\mathbb Q(\sqrt{-7})$, this is the character corresponding to $K$.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

For $K=\mathbb Q(\sqrt{-7})$,

$$
\zeta_K(s)=\zeta(s)L(s,\chi_3).
$$

The character is odd, $\chi_3(2)=1$, and

$$
\sum_{\substack{1\leq k<7/2\\(k,7)=1}}\chi_3(k)
=\chi_3(1)+\chi_3(2)+\chi_3(3)=1+1-1=1.
$$

The supplied odd-character formula gives

$$
L(1,\chi_3)=\frac{\pi}{\sqrt7}.
$$

The [analytic class number formula](../../../algebraic-number-theory.md#analytic-class-number-formula) for this imaginary quadratic field is

$$
\operatorname*{Res}_{s=1}\zeta_K(s)
=\frac{2\pi h_K}{w_K\sqrt{|d_K|}}
=\frac{\pi h_K}{\sqrt7},
$$

because $w_K=2$ and $d_K=-7$. Since $\operatorname*{Res}_{s=1}\zeta(s)=1$, comparison with $L(1,\chi_3)$ yields $\boxed{h_K=1}$.

## 4

↑ **Parent:** [Paper 123](paper-123.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [idele group](../../../algebraic-number-theory.md#idele-group) is the restricted product

$$
\mathbb I_K=\prod_v'K_v^\times
$$

over all places, with respect to $\mathcal O_v^\times$ at finite places. Thus an idele has a nonzero component in every completion and belongs to $\mathcal O_v^\times$ at all but finitely many finite places.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $\alpha=(\alpha_v)\in\mathbb I_K$, the congruence $\alpha\equiv1\pmod{\mathfrak m}$ means

$$
\alpha_\mathfrak p\in1+\mathfrak p^{n_\mathfrak p}\mathcal O_\mathfrak p
\quad(\mathfrak p\mid\mathfrak m_0),
\qquad
\alpha_v>0\quad(v\mid\mathfrak m_\infty).
$$

At finite primes outside the modulus require $\alpha_\mathfrak p\in\mathcal O_\mathfrak p^\times$. These ideles form $\mathbb I_K(\mathfrak m)$. Their image

$$
C_K(\mathfrak m)
=K^\times\mathbb I_K(\mathfrak m)/K^\times
$$

inside the [idèle class group](../../../algebraic-number-theory.md#idele-class-group) is the [idelic congruence subgroup](../../../algebraic-number-theory.md#idelic-congruence-subgroup).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write $m=\prod_pp^{n_p}$. For the modulus $m\infty$,

$$
\mathbb I_{\mathbb Q}(m\infty)
=\mathbb R_{>0}\times
\prod_{p\mid m}(1+p^{n_p}\mathbb Z_p)
\times\prod_{p\nmid m}\mathbb Z_p^\times.
$$

This is understood as the corresponding restricted-product subgroup of $\mathbb I_{\mathbb Q}$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Multiplying by a positive rational number normalizes the real component and all valuations, leaving the finite unit residue modulo $m$. This identifies

$$
C_{\mathbb Q}/C_{\mathbb Q}(m\infty)
\cong(\mathbb Z/m\mathbb Z)^\times.
$$

Locally,

$$
[\mathbb Z_p^\times:1+p^{n_p}\mathbb Z_p]
=p^{n_p-1}(p-1)
$$

when $n_p>0$. Multiplying gives

$$
\boxed{[C_{\mathbb Q}:C_{\mathbb Q}(m\infty)]
=\prod_{p\mid m}p^{n_p-1}(p-1)
=m\prod_{p\mid m}\left(1-\frac1p\right)
=\varphi(m).}
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The assumed inclusion and the class-field norm-index theorem give

$$
C_{\mathbb Q}(m\infty)
\subseteq N_{\mathbb Q(\zeta_m)/\mathbb Q}C_{\mathbb Q(\zeta_m)}
\subseteq C_{\mathbb Q}.
$$

The outer subgroup has index $\varphi(m)$ by part (d), while

$$
[C_{\mathbb Q}:N_{\mathbb Q(\zeta_m)/\mathbb Q}C_{\mathbb Q(\zeta_m)}]
=[\mathbb Q(\zeta_m):\mathbb Q]
=\varphi(m).
$$

Two nested subgroups of the same finite index are equal. Thus

$$
\boxed{C_{\mathbb Q}(m\infty)
=N_{\mathbb Q(\zeta_m)/\mathbb Q}C_{\mathbb Q(\zeta_m)}.}
$$

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

The [Kronecker–Weber theorem](../../../algebraic-number-theory.md#kronecker-weber-theorem) says that every finite abelian extension of $\mathbb Q$ lies in some $\mathbb Q(\zeta_m)$.

Indeed, global class field theory assigns to a finite abelian $L/\mathbb Q$ the open [norm group of an abelian extension](../../../algebraic-number-theory.md#norm-group-of-an-abelian-extension) $N_{L/\mathbb Q}C_L$. It contains a congruence subgroup $C_{\mathbb Q}(m\infty)$. By part (e), this is the norm group of $\mathbb Q(\zeta_m)$. The inclusion-reversing class-field correspondence therefore gives

$$
\boxed{L\subseteq\mathbb Q(\zeta_m).}
$$

## 5

↑ **Parent:** [Paper 123](paper-123.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a set $S$ of prime ideals, its [Dirichlet density](../../../algebraic-number-theory.md#dirichlet-density) is

$$
\delta(S)=\lim_{s\to1^+}
\frac{\sum_{\mathfrak p\in S}N\mathfrak p^{-s}}
{\log(1/(s-1))}
$$

when this limit exists.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $G=\operatorname{Cl}(K)$ and let $\widehat G$ be its character group. Character orthogonality gives

$$
\mathbf1_{[\mathfrak p]=C}
=\frac1{h_K}\sum_{\chi\in\widehat G}
\overline{\chi(C)}\,\chi([\mathfrak p]).
$$

For $\operatorname{Re}s>1$, the prime term of $\log L(s,\chi)$ is

$$
\sum_{\mathfrak p}\chi([\mathfrak p])N\mathfrak p^{-s},
$$

up to a function bounded as $s\to1^+$, since higher prime powers converge there. The trivial character contributes

$$
\log\frac1{s-1}+O(1),
$$

whereas every nontrivial character contributes $O(1)$ because its $L$-function is nonzero at $1$. Therefore

$$
\sum_{[\mathfrak p]=C}N\mathfrak p^{-s}
=\frac1{h_K}\log\frac1{s-1}+O(1),
$$

and the density is $\boxed{1/h_K}$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [Chebotarev density theorem](../../../algebraic-number-theory.md#chebotarev-density-theorem) states that for a finite Galois extension $L/K$ and a conjugacy class $C\subseteq\operatorname{Gal}(L/K)$, the unramified primes whose Frobenius conjugacy class is $C$ have Dirichlet density

$$
\boxed{\frac{|C|}{|\operatorname{Gal}(L/K)|}}.
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Put

$$
H=\mathbb Q(\sqrt2,\sqrt{13}).
$$

It contains $K=\mathbb Q(\sqrt{26})$ and has degree two over $K$. The three quadratic subfields have discriminants $8$, $13$, and $104$, so the biquadratic discriminant formula gives

$$
d_H=8\cdot13\cdot104=104^2=d_K^2.
$$

The relative discriminant formula

$$
d_H=d_K^{[H:K]}N_{K/\mathbb Q}(\mathfrak d_{H/K})
$$

therefore gives $\mathfrak d_{H/K}=\mathcal O_K$: no finite prime ramifies. The extension is totally real, so no infinite prime ramifies either. Since $h_K=2$, the [Hilbert class field](../../../algebraic-number-theory.md#hilbert-class-field) has degree two over $K$. Consequently

$$
\boxed{H_K=\mathbb Q(\sqrt2,\sqrt{13}).}
$$

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

A prime ideal of $K$ is principal exactly when its Artin symbol in

$$
\operatorname{Gal}(H_K/K)\cong\operatorname{Cl}(K)
$$

is the identity. The group has order two. Applying the [Chebotarev density theorem](../../../algebraic-number-theory.md#chebotarev-density-theorem) to the identity conjugacy class gives density

$$
\boxed{\frac12}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
