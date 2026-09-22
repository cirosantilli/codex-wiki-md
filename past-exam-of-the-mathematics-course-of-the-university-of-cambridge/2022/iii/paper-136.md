# Paper 136

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_136.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_136.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [inverse different](../../../arithmetic.md#inverse-different) is

$$
\mathfrak D_{L/K}^{-1}=\{x\in L:\operatorname{Tr}_{L/K}(x\mathcal O_L)\subseteq\mathcal O_K\}.
$$

It is an $\mathcal O_L$-submodule of $L$. Choose an integral basis $e_1,\ldots,e_n$ of a finite-index free submodule of $\mathcal O_L$. Nondegeneracy of the [trace pairing](../../../algebraic-number-theory.md#trace-form-of-a-number-field) gives a dual $K$-basis $e_1^*,\ldots,e_n^*$, and the codifferent lies between two finitely generated full $\mathcal O_K$-lattices obtained from these bases. It is therefore a fractional $\mathcal O_L$-ideal.

Every algebraic integer has integral trace, so $\mathcal O_L\subseteq\mathfrak D_{L/K}^{-1}$. Consequently its inverse

$$
\mathfrak D_{L/K}=\{y\in L:y\mathfrak D_{L/K}^{-1}\subseteq\mathcal O_L\}
$$

is contained in $\mathcal O_L$. It is thus an integral $\mathcal O_L$-ideal, called the [different ideal](../../../arithmetic.md#different-ideal).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Let $n=[L:K]$ and write $g(X)=\prod_{j=1}^n(X-\alpha_j)$. Lagrange interpolation, followed by summing over the conjugates, shows that the trace-dual of the power basis $1,\alpha,\ldots,\alpha^{n-1}$ is contained in $g'(\alpha)^{-1}\mathcal O_K[\alpha]$ and has the same determinant. Hence

$$
\mathfrak D_{L/K}^{-1}=\frac1{g'(\alpha)}\mathcal O_L,
\qquad
\mathfrak D_{L/K}=(g'(\alpha)).
$$

For $L=\mathbb Q(\sqrt3)$, the [ring of integers of a quadratic field](../../../algebraic-number-theory.md#ring-of-integers-of-a-quadratic-field) is $\mathbb Z[\sqrt3]$. Taking $g=X^2-3$ gives

$$
\mathfrak D_{L/\mathbb Q}=(2\sqrt3).
$$

For $L=\mathbb Q(\sqrt5)$, use $\alpha=(1+\sqrt5)/2$ and $g=X^2-X-1$. Then

$$
\mathfrak D_{L/\mathbb Q}=(2\alpha-1)=(\sqrt5).
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The ring $\mathbb Z[T]$ is Noetherian and integrally closed, but it is not a [Dedekind domain](../../../commutative-algebra.md#dedekind-domain) because it has Krull dimension two. Concretely, the nonzero prime ideal $(2)$ is properly contained in the prime ideal $(2,T)$ and is therefore not maximal.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The element $T$ belongs to the fraction field of $R=\mathbb C[T^2,T^3]$ and is integral over $R$, since it satisfies the monic polynomial $X^2-T^2$. But $T\notin R$. Thus $R$ is not [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain) and hence is not a Dedekind domain.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The ring $\mathbb Z[\zeta_3]$ is the full ring of integers of the [quadratic number field](../../../algebraic-number-theory.md#quadratic-field) $\mathbb Q(\sqrt{-3})$. Every ring of integers of a number field is a Dedekind domain, so this ring is Dedekind.

## 2

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Suppose first that the valuation is discrete and the residue field $k$ is finite. For a uniformizer $\pi$, every quotient $\mathcal O_K/\pi^n\mathcal O_K$ is finite, and completeness gives

$$
\mathcal O_K\cong\varprojlim_n\mathcal O_K/\pi^n\mathcal O_K.
$$

This inverse limit is compact. Since $\mathcal O_K$ is a compact neighborhood of zero, $K$ is locally compact.

Conversely, local compactness gives a compact ball about zero, which can be rescaled to make $\mathcal O_K$ compact. Its distinct residue classes are disjoint open balls of radius below one, so compactness forces the residue field to be finite. Cover $\mathcal O_K$ by finitely many balls of some radius $r<1$. Applying the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) to centers lying in the maximal ideal produces $\rho<1$ such that every nonunit has absolute value at most $\rho$. Hence the value group has a largest value below one, and the valuation is discrete. This proves the [local compactness criterion for a complete non-Archimedean field](../../../arithmetic.md#local-compactness-criterion-for-a-complete-non-archimedean-field).

An algebraically closed valued field has an $n$th root of every element. If its valuation were discrete and $\pi$ were a uniformizer, then $v(\sqrt[n]{\pi})=1/n$ would contradict discreteness. Therefore an algebraically closed non-Archimedean field cannot be locally compact.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

If $|\cdot|$ is non-Archimedean, then $|n|=|1+\cdots+1|\leq1$. Conversely suppose $|n|\leq M$ for every integer $n$. The binomial theorem and the ordinary triangle inequality give

$$
|x+y|^N\leq (N+1)M\max(|x|,|y|)^N.
$$

Taking $N$th roots and letting $N\to\infty$ proves $|x+y|\leq\max(|x|,|y|)$. This is the [bounded-integer criterion for a non-Archimedean absolute value](../../../arithmetic.md#bounded-integer-criterion-for-a-non-archimedean-absolute-value).

In characteristic $p$, the image of $\mathbb Z$ is the finite prime field $\mathbb F_p$, so every absolute value is bounded on it. Thus every absolute value on $\mathbb F_p(t)$ is non-Archimedean.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The polynomial

$$
h(t)=t^3-t-1\in\mathbb F_3[t]
$$

has no root in $\mathbb F_3$ and is therefore irreducible. Define

$$
\left|\frac{a(t)}{b(t)}\right|_h
=c^{\operatorname{ord}_h(b)-\operatorname{ord}_h(a)}
$$

for any fixed $c>1$. Its valuation ring has residue field

$$
\mathbb F_3[t]/(h)\cong\mathbb F_{27}.
$$

The [completion at an irreducible polynomial over a finite field](../../../arithmetic.md#completion-at-an-irreducible-polynomial-over-a-finite-field) identifies the completion with $\mathbb F_{27}((T))$, where $T$ corresponds to the uniformizer $h(t)$.

## 3

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\mathfrak m_K$ be the maximal ideal. For all sufficiently large $r$, the convergent [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) and [p-adic exponential](../../../arithmetic.md#p-adic-exponential-function) give the [principal-unit logarithm](../../../arithmetic.md#principal-unit-logarithm) isomorphism

$$
1+\mathfrak m_K^r\xrightarrow{\ \log\ }(\mathfrak m_K^r,+).
$$

Multiplication by a power of a uniformizer identifies the additive group $\mathfrak m_K^r$ with $(\mathcal O_K,+)$. Since $1+\mathfrak m_K^r$ has finite index in $\mathcal O_K^\times$, it is the required subgroup.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $\alpha=\sqrt[p]{p}$. The polynomial $X^p-p$ is [Eisenstein](../../../arithmetic.md#eisenstein-polynomial), so $\mathbb Q_p(\alpha)/\mathbb Q_p$ is totally ramified of degree $p$. The cyclotomic extension $\mathbb Q_p(\zeta_p)/\mathbb Q_p$ is totally ramified of degree $p-1$. Their coprime degrees make their intersection trivial, so

$$
K=\mathbb Q_p(\zeta_p,\alpha)
$$

has degree $p(p-1)$ and is totally ramified. It is the splitting field of $X^p-p$, hence Galois.

Normalize $v_K$ by $v_K(K^\times)=\mathbb Z$. Then

$$
v_K(\zeta_p-1)=p,
\qquad v_K(\alpha)=p-1,
$$

so

$$
\varpi=\frac{\zeta_p-1}{\alpha}
$$

is a [uniformizer](../../../commutative-algebra.md#uniformizer). Write an automorphism as

$$
\sigma_{a,b}(\zeta_p)=\zeta_p^a,
\qquad
\sigma_{a,b}(\alpha)=\zeta_p^b\alpha,
$$

where $a\in\mathbb F_p^\times$ and $b\in\mathbb F_p$. Since

$$
\frac{\sigma_{a,b}(\varpi)}{\varpi}
=\zeta_p^{-b}\frac{\zeta_p^a-1}{\zeta_p-1},
$$

the [uniformizer criterion for lower ramification groups](../../../arithmetic.md#uniformizer-criterion-for-lower-ramification-groups) gives valuation one for $\sigma(\varpi)-\varpi$ when $a\ne1$, and valuation $p+1$ when $a=1$, $b\ne0$. Therefore

$$
G_0=G,qquad
G_i=\{\sigma_{1,b}:b\in\mathbb F_p\}\cong\mathbb Z/p\mathbb Z\quad(1\leq i\leq p),
$$

and $G_i=1$ for $i\geq p+1$. These are the [ramification groups of the splitting field of Xp minus p over the p-adic numbers](../../../arithmetic.md#ramification-groups-of-the-splitting-field-of-xp-minus-p-over-the-p-adic-numbers).

## 4

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

One strong form of the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) is this: if a complete discretely valued field $K$, a polynomial $f\in\mathcal O_K[X]$, and $a\in\mathcal O_K$ satisfy

$$
v(f(a))>2v(f'(a)),
$$

then there is a unique root $\alpha$ in the ball $v(\alpha-a)>v(f'(a))$.

Set $a_{n+1}=a_n-f(a_n)/f'(a_n)$. Taylor expansion shows that the valuation of the error at least doubles at each step, while $v(f'(a_n))$ remains constant. Thus the corrections tend to zero geometrically, so completeness gives a limit $\alpha$. Continuity gives $f(\alpha)=0$. Applying the same Taylor estimate to two roots in the stated ball proves uniqueness. This is [Newton iteration over a valued field](../../../arithmetic.md#newton-iteration-over-a-valued-field).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $x=\pi^ru$ with $r\in\mathbb Z$ and $u\in\mathcal O_K^\times$. If $x$ is an $m$th power, then $m$ divides $r$. Divisibility by infinitely many $m$ forces $r=0$, so $x$ is a unit.

Conversely, if $m$ is coprime to both the residue characteristic $p$ and $q-1$, exponentiation by $m$ is an automorphism on the finite residue-unit group and on every [principal unit](../../../arithmetic.md#principal-unit) quotient; equivalently, use Hensel's lemma on $Y^m-u$. Hence every unit is an $m$th power for infinitely many such $m$. Therefore

$$
P=\mathcal O_K^\times,
$$

as recorded by [elements that are powers of infinitely many degrees in a local field](../../../arithmetic.md#elements-that-are-powers-of-infinitely-many-degrees-in-a-local-field).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $Y=X^2$. Modulo two, $Y^2+9Y-2$ has the two simple roots zero and one, so [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) lifts them to roots $y_0,y_1\in\mathbb Z_2$, with $v_2(y_0)=1$ and $y_1\equiv1\pmod8$. The [2-adic unit](../../../arithmetic.md#2-adic-unit) criterion makes $y_1$ a square, so $X^2-y_1$ splits into two linear factors. The polynomial $X^2-y_0$ is Eisenstein and remains irreducible. Thus $X^4+9X^2-2$ has three irreducible factors, of degrees $1,1,2$, as in [factorization of X4 plus 9X2 minus 2 over the 2-adic numbers](../../../arithmetic.md#factorization-of-x4-plus-9x2-minus-2-over-the-2-adic-numbers).

## 5

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Seek $F=L+F_2+F_3+\cdots$, with each $F_d$ homogeneous of degree $d$. Suppose the terms below degree $d$ have been chosen. Comparing degree $d$ in

$$
f(F(X_1,\ldots,X_n))=F(g(X_1),\ldots,g(X_n))
$$

gives a linear equation for $F_d$ whose coefficient is $\pi-\pi^d=\pi(1-\pi^{d-1})$. The already known term is divisible by $\pi$ because $f(X),g(X)\equiv X^q\pmod\pi$ and every residue $\bar a_i\in\mathbb F_q$ satisfies $\bar a_i^q=\bar a_i$. Since $1-\pi^{d-1}$ is a unit, this determines a unique integral $F_d$. Induction constructs a unique $F\in\mathcal O_K[[X_1,\ldots,X_n]]$. This is the [Lubin–Tate functional equation lemma](../../../arithmetic.md#lubin-tate-functional-equation-lemma).

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

Take $f=g$ and $L=X_1+\cdots+X_n$. Permuting the variables produces another solution with the same linear term, so uniqueness gives

$$
F(X_1,\ldots,X_n)=F(X_{\sigma(1)},\ldots,X_{\sigma(n)}).
$$

For $a\in\mathcal O_K$, the one-variable case of part i gives a unique $\theta_a(X)\equiv aX\pmod{X^2}$ commuting with $f$. Applying uniqueness once more to the two ways of composing $\theta_a$ with $F$ gives

$$
\theta_a(F(X_1,\ldots,X_n))
=F(\theta_a(X_1),\ldots,\theta_a(X_n)).
$$

**Thus $F$ is the addition law and the $\theta_a$ are scalar endomorphisms of the [Lubin–Tate formal group](../../../arithmetic.md#lubin-tate-formal-group).**

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Since $f(X)=X(\pi+X^{q-1})$, its iterates satisfy

$$
\Phi_m(X):=\frac{f_m(X)}{f_{m-1}(X)}
=\pi+f_{m-1}(X)^{q-1}.
$$

The polynomial $\Phi_m$ is [Eisenstein](../../../arithmetic.md#eisenstein-polynomial): it is monic, every nonleading coefficient is divisible by $\pi$, and its constant term is $\pi$. It is also separable, since $q-1$ is prime to the residue characteristic and the iterates have nonzero derivative.

If $\alpha\ne0$ and $m$ is least with $f_m(\alpha)=0$, then $\Phi_m(\alpha)=0$. Eisenstein irreducibility makes $\Phi_m$ its minimal polynomial, so $K(\alpha)/K$ is totally ramified and separable. For $\alpha=0$ the extension is trivial and has the same properties. This is the [Eisenstein layers of Lubin–Tate torsion](../../../arithmetic.md#eisenstein-layers-of-lubin-tate-torsion) argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
