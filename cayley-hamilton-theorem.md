# Cayley-Hamilton theorem

↑ **Parent:** [Minimal polynomial](linear-operator-theory.md#minimal-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley-Hamilton_theorem)

Every [square matrix](vector-space.md#square-matrix) satisfies its own [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial). More explicitly, for an $n$-by-$n$ [matrix](vector-space.md#matrix) $A$ over a [commutative ring](commutative-algebra.md#commutative-ring) with identity, form

$$
\chi_A(t)=\det(tI-A)=t^n+c_{n-1}t^{n-1}+\cdots+c_1t+c_0.
$$

Then

$$
\boxed{A^n+c_{n-1}A^{n-1}+\cdots+c_1A+c_0I=0.}
$$

Here $0$ is the [zero matrix](vector-space.md#zero-matrix), and the constant term multiplies the [identity matrix](vector-space.md#identity-matrix). This is a [polynomial evaluated at a matrix](#polynomial-evaluated-at-a-matrix); it is stronger than saying that each [eigenvalue](linear-operator-theory.md#eigenvalue) is a [root of a polynomial](polynomial.md#root-of-a-polynomial). Neither [diagonalizability](linear-operator-theory.md#diagonalizable-matrix) nor distinct [eigenvalues](linear-operator-theory.md#eigenvalue) is required.[§3, Theorem 3.4 and the universal-identity discussion, printed pp. 6–7: matrices over arbitrary commutative rings](mathematics-bibliography.md#universal-identities-by-keith-conrad)

The practical payoff is that arbitrarily high [matrix powers](vector-space.md#matrix-power) can be reduced to a combination of $I,A,\ldots,A^{n-1}$. These powers arise when repeatedly applying a [linear map](vector-space.md#linear-map), solving a [linear recurrence relation](algebra.md#linear-recurrence-relation), or evolving a finite [state space](dynamical-systems.md#state-space) model. The [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) turns that repeated action into a fixed-order scalar recurrence. The [minimal polynomial](linear-operator-theory.md#minimal-polynomial) may reduce the number of required powers further.

**Table of contents**

- [Polynomial evaluated at a matrix](#polynomial-evaluated-at-a-matrix)
- [Two-coefficient reduction of matrix powers](#two-coefficient-reduction-of-matrix-powers)
- [Polynomial reduction of matrix powers](#polynomial-reduction-of-matrix-powers)
- [Repeated eigenvalues in the Cayley-Hamilton theorem](#repeated-eigenvalues-in-the-cayley-hamilton-theorem)
- [Cayley's matrix memoir](#cayley-s-matrix-memoir)
- [Cayley-Hamilton theorem from cyclic subspaces](#cayley-hamilton-theorem-from-cyclic-subspaces)

## Polynomial evaluated at a matrix

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem.md)

For a [polynomial](polynomial.md) $p(t)=\sum_{j=0}^d a_jt^j$, substitute a fixed [square matrix](vector-space.md#square-matrix) $A$ for $t$, taking $A^0=I$. In particular, $p(t)=t^2-3t+1$ becomes $p(A)=A^2-3A+I$, not $A^2-3A$ with the scalar $1$ added separately to each entry. [Polynomials](polynomial.md) in the same [matrix](vector-space.md#matrix) commute with each other, even though arbitrary [matrix multiplication](vector-space.md#matrix-multiplication) is [noncommutative](algebraic-operation.md#noncommutativity).

## Two-coefficient reduction of matrix powers

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem.md)

Consider the real [matrix](vector-space.md#matrix)

$$
A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad
\chi_A(t)=(t-2)(t-1)-1=t^2-3t+1.
$$

The [Cayley-Hamilton theorem](cayley-hamilton-theorem.md) gives $A^2=3A-I$. Consequently

$$
A^3=3A^2-A=8A-3I,\qquad
A^4=21A-8I,\qquad A^5=55A-21I.
$$

Thus

$$
\boxed{A^5=\begin{pmatrix}89&55\\55&34\end{pmatrix}.}
$$

All four entries come from just two scalar coefficients. If $A^n=a_nA+b_nI$, multiplying once by $A$ and replacing $A^2$ gives the [linear recurrence relation](algebra.md#linear-recurrence-relation)

$$
a_{n+1}=3a_n+b_n,\qquad b_{n+1}=-a_n,
\qquad(a_0,b_0)=(0,1).
$$

Equivalently $a_{n+2}=3a_{n+1}-a_n$, with $a_0=0,a_1=1$. The appearance of [Fibonacci numbers](sequence-and-series.md#fibonacci-number) is explained by $A=Q^2$, where $Q=\begin{pmatrix}1&1\\1&0\end{pmatrix}$ advances the [Fibonacci recurrence](sequence-and-series.md#fibonacci-recurrence). No [eigenvectors](linear-operator-theory.md#eigenvector) need to be computed.

<a id="image-cayley-hamilton-reduces-powers-of-a-chosen-two-by-two-matrix-to-two-integer-coefficients-the-fifth-power-is-55a-minus-21i"></a>
![](cayley-hamilton-matrix-power-reduction.png)

**[Figure 1](#image-cayley-hamilton-reduces-powers-of-a-chosen-two-by-two-matrix-to-two-integer-coefficients-the-fifth-power-is-55a-minus-21i). Cayley–Hamilton reduces powers of a chosen two-by-two matrix to two integer coefficients; the fifth power is 55A − 21I**.

The same identity computes an inverse. Rearrange it as $A(3I-A)=I$, giving

$$
\boxed{A^{-1}=3I-A=\begin{pmatrix}1&-1\\-1&2\end{pmatrix}.}
$$

This works because the constant term of this [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is nonzero and the coefficients lie in a [field](algebra.md#field). Generally, when $c_0\ne0$ over a [field](algebra.md#field), rearranging the [Cayley-Hamilton theorem](cayley-hamilton-theorem.md) expresses $A^{-1}$ as a [polynomial evaluated at a matrix](#polynomial-evaluated-at-a-matrix). Over a general [commutative ring](commutative-algebra.md#commutative-ring), a nonzero constant need not be a [unit](algebra.md#unit-in-a-ring); invertibility requires that extra condition.

## Polynomial reduction of matrix powers

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem.md)

By [polynomial division](polynomial.md#polynomial-division), write $f(t)=q(t)\chi_A(t)+r(t)$ with $\deg r<n$. Because $\chi_A$ is a [monic polynomial](polynomial.md#monic-polynomial), this division works even over a [commutative ring](commutative-algebra.md#commutative-ring). Evaluating at $A$ makes the multiple of $\chi_A(A)$ vanish, leaving $f(A)=r(A)$. This explains the reduction in [two-coefficient reduction of matrix powers](#two-coefficient-reduction-of-matrix-powers) without multiplying out every intermediate [matrix](vector-space.md#matrix).

Over a [field](algebra.md#field), the [minimal polynomial](linear-operator-theory.md#minimal-polynomial) $m_A$ divides $\chi_A$ and gives the strongest such universal reduction: use the [polynomial remainder](polynomial.md#remainder-of-polynomial-division) modulo $m_A$ instead. For the [scalar matrix](linear-algebra.md#scalar-matrix) $2I_2$, the [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is $(t-2)^2$, while the [minimal polynomial](linear-operator-theory.md#minimal-polynomial) is only $t-2$. Every [matrix power](vector-space.md#matrix-power) is then a scalar multiple of $I_2$.

## Repeated eigenvalues in the Cayley-Hamilton theorem

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem.md)

Take a different real [matrix](vector-space.md#matrix),

$$
B=\begin{pmatrix}2&1\\0&2\end{pmatrix}=2I+N,
\qquad N=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
$$

Its only [eigenvalue](linear-operator-theory.md#eigenvalue) is $2$, with [algebraic multiplicity](linear-operator-theory.md#algebraic-multiplicity) two. However, the [polynomial](polynomial.md) $q(t)=t-2$, which vanishes at that [eigenvalue](linear-operator-theory.md#eigenvalue), gives $q(B)=N\ne0$. Merely checking values at [eigenvalues](linear-operator-theory.md#eigenvalue) cannot prove a matrix identity. The full [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) does work:

$$
\chi_B(t)=(t-2)^2,\qquad \chi_B(B)=N^2=0.
$$

The [matrix](vector-space.md#matrix) is a [Jordan block](linear-operator-theory.md#jordan-block), and its [minimal polynomial](linear-operator-theory.md#minimal-polynomial) is also $(t-2)^2$.

The [binomial theorem](binomial-coefficient.md#binomial-theorem) gives, for positive [integers](integer.md) $n$,

$$
\boxed{B^n=2^nI+n2^{n-1}N.}
$$

Terms containing $N^2$ or a higher [matrix power](vector-space.md#matrix-power) vanish. After removing the common growth factor $2^n$, the remaining [linear map](vector-space.md#linear-map) is the [shear mapping](vector-space.md#shear-mapping) $I+(n/2)N$. It moves $(x,y)$ to $(x+ny/2,y)$. The single [eigenvalue](linear-operator-theory.md#eigenvalue) controls the exponential scale, while the [nilpotent matrix](linear-operator-theory.md#nilpotent-matrix) adds a factor growing linearly in $n$.

<a id="image-normalized-powers-of-a-jordan-block-retain-a-growing-shear-despite-having-only-one-eigenvalue-equal-axes-scales-show-the-top-edge-moving-by-n-2"></a>
![](cayley-hamilton-jordan-block-shear.png)

**[Figure 2](#image-normalized-powers-of-a-jordan-block-retain-a-growing-shear-despite-having-only-one-eigenvalue-equal-axes-scales-show-the-top-edge-moving-by-n-2). Normalized powers of a Jordan block retain a growing shear despite having only one eigenvalue; equal axes scales show the top edge moving by n/2**.

In terms of [polynomial interpolation](interpolation.md#polynomial-interpolation), reduction modulo $(t-2)^2$ retains both a value and a [derivative](calculus.md#derivative):

$$
f(B)=f(2)I+f'(2)N.
$$

Indeed, [polynomial division](polynomial.md#polynomial-division) gives $f(t)=f(2)+f'(2)(t-2)+(t-2)^2h(t)$. This is a simple [Hermite interpolation](algebra.md#hermite-interpolation) condition. For $f(t)=t^n$, it gives exactly the displayed [matrix power](vector-space.md#matrix-power). Repeated [eigenvalues](linear-operator-theory.md#eigenvalue) retain information about how a [polynomial](polynomial.md) changes, not just where it vanishes.

<h2 id="cayley-s-matrix-memoir">Cayley's matrix memoir</h2>

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem.md)

[Arthur Cayley](mathematics-author.md#arthur-cayley)'s 1858 paper A Memoir on the Theory of Matrices motivates [matrices](vector-space.md#matrix) as an abbreviated way to write [systems of linear equations](linear-algebra.md#system-of-linear-equations). Its opening already connects the characteristic equation with reducing [polynomials](polynomial.md) in a [matrix](vector-space.md#matrix) to lower degree. In §21 he works out the two-by-two identity; in §23 he says he has verified the three-by-three case but does not give a formal proof for every size. Thus this source distinguishes the general statement from a general proof.[Printed pp. 17–18, opening motivation; pp. 23–24, §§21–25, characteristic equation and reduction of matrix functions; received 10 December 1857, read 14 January 1858, published 1858](mathematics-bibliography.md#a-memoir-on-the-theory-of-matrices-by-arthur-cayley) The theorem's name also commemorates [William Rowan Hamilton](mathematics-author.md#william-rowan-hamilton).

## Cayley-Hamilton theorem from cyclic subspaces

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem.md)

Over a [field](algebra.md#field), a [cyclic vector](linear-operator-theory.md#cyclic-vector) gives a [companion matrix](linear-operator-theory.md#companion-matrix), whose characteristic relation annihilates its generator and hence every iterate. If there is no [cyclic vector](linear-operator-theory.md#cyclic-vector) spanning the whole space, a nonzero proper [cyclic subspace](linear-operator-theory.md#cyclic-subspace) is invariant. Induction annihilates the restriction and the quotient; the quotient polynomial first sends the whole space into the invariant subspace, and the restriction polynomial then kills it. The block-triangular [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is the product of these two polynomials.

## ↑ Ancestors (7)

1. [Minimal polynomial](linear-operator-theory.md#minimal-polynomial)
2. [Operator theory](linear-operator-theory.md)
3. [Linear algebra](linear-algebra.md)
4. [Algebra](algebra.md)
5. [Area of mathematics](mathematics.md#area-of-mathematics)
6. [Mathematics](mathematics.md)
7. [Codex Wiki](README.md)

## ← Incoming links (44)

- [Automorphism of a one-dimensional complex torus](complex-geometry.md#automorphism-of-a-one-dimensional-complex-torus)
- [Cyclic subspace](linear-operator-theory.md#cyclic-subspace)
- [Minimal polynomial](linear-operator-theory.md#minimal-polynomial)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3.md#1f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3.md#5f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2.md#15g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1.md#22h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3.md#13e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4.md#11e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#10g/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#10g/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1.md#7a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#24h/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1.md#7b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1.md#9g/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#16h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#19h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#31a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3.md#10e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-1.md#7b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#23f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1.md#9g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1.md#6a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1.md#6a/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#20g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1.md#8b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3.md#9f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1.md#6c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#8f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1.md#6c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1.md#5/solution)
- [Real special linear group of degree two](group-theory.md#real-special-linear-group-of-degree-two)
- [Rotational invariant of a symmetric traceless tensor](critical-phenomenon.md#rotational-invariant-of-a-symmetric-traceless-tensor)
- [Scalar square of a traceless two-by-two matrix](linear-algebra.md#scalar-square-of-a-traceless-two-by-two-matrix)
- [Square-zero criterion for a two-by-two matrix](linear-operator-theory.md#square-zero-criterion-for-a-two-by-two-matrix)
- [Two-coefficient reduction of matrix powers](#two-coefficient-reduction-of-matrix-powers)
