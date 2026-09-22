<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A precise version of the [Hilbert-Serre theorem](../../../../../hilbert-serre-theorem.md) is as follows. Let $R=\bigoplus_{j\ge0}R_j$ be a commutative [graded ring](../../../../../graded-ring.md), generated over an [Artinian](../../../../../artinian-ring.md) degree-zero ring $R_0$ by homogeneous elements $y_1,\ldots,y_s$ of positive degrees $d_1,\ldots,d_s$. Let $M$ be a finitely generated [graded module](../../../../../graded-module.md), bounded below. Each component has finite [module length](../../../../../length-of-a-module.md) over $R_0$. Its [Poincare series of a graded module](../../../../../poincare-series-of-a-graded-module.md), or [Hilbert series](../../../../../hilbert-series.md), is

$$
P_M(t)=\sum_j\ell_{R_0}(M_j)t^j.
$$

When $R_0$ is a field, these lengths are dimensions. The theorem asserts

$$
\boxed{P_M(t)=\frac{q(t)}{\prod_{i=1}^s(1-t^{d_i})},\qquad q(t)\in\mathbb Z[t,t^{-1}].}
$$

For a nonnegatively graded module the numerator can be taken in $\mathbb Z[t]$. The finite-generation and finite-length hypotheses specify the meaning of the series; they are part of the theorem's statement.

We prove it by induction on $s$. Regard $M$ as a finite graded module over $S=R_0[Y_1,\ldots,Y_s]$, with $\deg Y_i=d_i$, acting through the specified generators of $R$. This polynomial ring is [Noetherian](../../../../../noetherian-ring.md) by the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md) and Question 1. When $s=0$, finitely many homogeneous generators over $R_0$ mean that only finitely many components are nonzero, so the series is a Laurent polynomial. For the induction step, put $y=Y_s$, $d=d_s$, $K=(0:_M y)$ and $C=M/yM$. Both $K$ and $C$ are finite graded modules; $y$ annihilates them, so they are modules over $R_0[Y_1,\ldots,Y_{s-1}]$. The finite generation of $K$ uses Noetherianity of $S$.

The [exact sequence](../../../../../exact-sequence.md) of graded modules

$$
0\longrightarrow K(-d)\longrightarrow M(-d)
\xrightarrow{\ y\ }M\longrightarrow C\longrightarrow0
$$

gives, by additivity of component lengths,

$$
(1-t^d)P_M(t)=P_C(t)-t^dP_K(t).
$$

Here the shift is defined so that $P_{M(-d)}=t^dP_M$. By induction both series on the right have denominator $\prod_{i<s}(1-t^{d_i})$. Dividing by $1-t^d$ proves the result. The annihilator term cannot be omitted unless multiplication by $y$ is injective.

In the standard grading $d_i=1$, the coefficients of $(1-t)^{-s}$ are $\binom{j+s-1}{s-1}$. Multiplying by the finite numerator shows that the component dimensions agree with a polynomial for sufficiently large $j$. Cumulative dimensions have generating function $P_M(t)/(1-t)$ and are also eventually polynomial. This consequence supplies the dimension used for [Weyl algebra](../../../../../weyl-algebra.md) modules.

Use the [Bernstein filtration](../../../../../bernstein-filtration.md) $B_mA_n$, in which both coordinate generators and differentiation generators have degree one. The [ordered monomial basis of a Weyl algebra](../../../../../ordered-monomial-basis-of-a-weyl-algebra.md) gives

$$
\operatorname{gr}_B A_n\cong\mathbb C[x_1,\ldots,x_n,\xi_1,\ldots,\xi_n],\qquad
\dim_\mathbb C B_mA_n=\binom{m+2n}{2n}.
$$

Choose a finite-dimensional generating subspace $M_0$ of a nonzero finitely generated left module $M$ and set $M_m=B_mA_nM_0$. This is a [good filtration of a module](../../../../../good-filtration-of-a-module.md): the symbols of the generators generate its [associated graded module](../../../../../associated-graded-module.md) over the displayed polynomial ring. The [Hilbert-Serre theorem](../../../../../hilbert-serre-theorem.md) makes $\dim_\mathbb C M_m$ an eventual polynomial. Define the [Bernstein growth dimension of a Weyl algebra module](../../../../../bernstein-growth-dimension-of-a-weyl-algebra-module.md) by

$$
\boxed{d(M)=\deg\bigl(\dim_\mathbb C M_m\text{ for }m\gg0\bigr).}
$$

The dimension is independent of the chosen finite generating subspace. Each of two finite generating sets is contained in a fixed filtration step for the other, giving $M_m\subseteq M'_{m+c}$ and $M'_m\subseteq M_{m+c'}$. Such fixed shifts preserve the degree of growth. The same argument applies to any good Bernstein filtration. This dimension agrees with the [Gelfand–Kirillov dimension of a module](../../../../../gelfand-kirillov-dimension-of-a-module.md); one may set $d(0)=-\infty$.

Let the nonconstant element $D$ have Bernstein degree $d\ge1$. Since $\operatorname{gr}_B A_n$ is a domain, the product of two nonzero symbols cannot vanish. Hence

$$
\deg_B(aD)=\deg_B a+d\quad(a\ne0),\qquad
(A_nD)\cap B_mA_n=(B_{m-d}A_n)D.
$$

Right multiplication by $D$ is injective, using the domain property of $A_n$. Thus the quotient filtration on $M=A_n/A_nD$ has cumulative dimensions

$$
\dim_\mathbb C M_m=
\binom{m+2n}{2n}-\binom{m-d+2n}{2n}\quad(m\ge d).
$$

The leading terms of degree $2n$ cancel, and the leading surviving term is

$$
\frac{d}{(2n-1)!}\,m^{2n-1}.
$$

It is nonzero, because $d\ge1$. Therefore

$$
\boxed{d(A_n/A_nD)=2n-1.}
$$

Equivalently the [Hilbert series](../../../../../hilbert-series.md) of the associated graded quotient is $(1-t^d)/(1-t)^{2n}$. Here $d$ is Bernstein degree, not differential order: multiplication by $x_1$ has differential order zero but Bernstein degree one. Using the order filtration in this dimension argument would lose the finite-dimensional filtration pieces.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
