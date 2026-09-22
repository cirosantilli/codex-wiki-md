# Cayley-Hamilton theorem

↑ **Parent:** [Minimal polynomial](minimal-polynomial.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley-Hamilton_theorem)

Every [square matrix](square-matrix.md) satisfies its own [characteristic polynomial](characteristic-polynomial.md). More explicitly, for an $n$-by-$n$ [matrix](matrix.md) $A$ over a [commutative ring](commutative-ring.md) with identity, form

$$
\chi_A(t)=\det(tI-A)=t^n+c_{n-1}t^{n-1}+\cdots+c_1t+c_0.
$$

Then

$$
\boxed{A^n+c_{n-1}A^{n-1}+\cdots+c_1A+c_0I=0.}
$$

Here $0$ is the [zero matrix](zero-matrix.md), and the constant term multiplies the [identity matrix](identity-matrix.md). This is a [polynomial evaluated at a matrix](polynomial-evaluated-at-a-matrix.md); it is stronger than saying that each [eigenvalue](eigenvalue.md) is a [root of a polynomial](root-of-a-polynomial.md). Neither [diagonalizability](diagonalizable-matrix.md) nor distinct [eigenvalues](eigenvalue.md) is required.[§3, Theorem 3.4 and the universal-identity discussion, printed pp. 6–7: matrices over arbitrary commutative rings](universal-identities-by-keith-conrad.md)

The practical payoff is that arbitrarily high [matrix powers](matrix-power.md) can be reduced to a combination of $I,A,\ldots,A^{n-1}$. These powers arise when repeatedly applying a [linear map](linear-map.md), solving a [linear recurrence relation](linear-recurrence-relation.md), or evolving a finite [state space](state-space.md) model. The [characteristic polynomial](characteristic-polynomial.md) turns that repeated action into a fixed-order scalar recurrence. The [minimal polynomial](minimal-polynomial.md) may reduce the number of required powers further.

**Table of contents**

- [Polynomial evaluated at a matrix](polynomial-evaluated-at-a-matrix.md)
- [Two-coefficient reduction of matrix powers](two-coefficient-reduction-of-matrix-powers.md)
- [Polynomial reduction of matrix powers](polynomial-reduction-of-matrix-powers.md)
- [Repeated eigenvalues in the Cayley-Hamilton theorem](repeated-eigenvalues-in-the-cayley-hamilton-theorem.md)
- [Cayley's matrix memoir](cayley-s-matrix-memoir.md)
- [Cayley-Hamilton theorem from cyclic subspaces](cayley-hamilton-theorem-from-cyclic-subspaces.md)

## ↑ Ancestors (7)

1. [Minimal polynomial](minimal-polynomial.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (44)

- [Automorphism of a one-dimensional complex torus](automorphism-of-a-one-dimensional-complex-torus.md)
- [Cyclic subspace](cyclic-subspace.md)
- [Minimal polynomial](minimal-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/5f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/15g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-15/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/22h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/13e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/11e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/10g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/10g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/7a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/24h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/7b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/9g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/16h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/19h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/31a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-1/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/23f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/9g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/6a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/6a/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/20g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-3/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1/6c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1/6c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/5/solution.md)
- [Real special linear group of degree two](real-special-linear-group-of-degree-two.md)
- [Rotational invariant of a symmetric traceless tensor](rotational-invariant-of-a-symmetric-traceless-tensor.md)
- [Scalar square of a traceless two-by-two matrix](scalar-square-of-a-traceless-two-by-two-matrix.md)
- [Square-zero criterion for a two-by-two matrix](square-zero-criterion-for-a-two-by-two-matrix.md)
- [Two-coefficient reduction of matrix powers](two-coefficient-reduction-of-matrix-powers.md)
