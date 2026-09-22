<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First apply the [commutator product rule](../../../../../commutator-product-rule.md) in the form $[AB,C]=A[B,C]+[A,C]B$:

$$
[N,a_j^*]=\sum_{k=1}^2\left(a_k^*[a_k,a_j^*]+[a_k^*,a_j^*]a_k\right)=a_j^*.
$$

Repeated use of the [commutator product rule](../../../../../commutator-product-rule.md) gives, for $n\geq1$,

$$
[N,(a_j^*)^n]=\sum_{r=0}^{n-1}(a_j^*)^r[N,a_j^*](a_j^*)^{n-1-r}
=n(a_j^*)^n.
$$

This is the [commutator with powers of an eigenoperator](../../../../../commutator-with-powers-of-an-eigenoperator.md). For $n=0$, the [commutator](../../../../../commutator.md) with the [identity operator](../../../../../identity-operator.md) is zero, agreeing with the formula.

Each $a_k^*a_k$ is unchanged by taking the [adjoint operator](../../../../../adjoint-operator.md), so $N^*=N$ in this algebra. Taking the [adjoint of a commutator](../../../../../adjoint-of-a-commutator.md) yields $[N,(a_j^*)^n]^*=[a_j^n,N]=na_j^n$. By antisymmetry,

$$
\boxed{[N,(a_j^*)^n]=n(a_j^*)^n,\qquad [N,a_j^n]=-na_j^n,\qquad n=0,1,2,\ldots.}
$$

In particular, each [creation operator](../../../../../creation-operator.md) raises the [number operator](../../../../../number-operator.md) [eigenvalue](../../../../../eigenvalue.md) by one, and each [annihilation operator](../../../../../annihilation-operator.md) lowers it by one.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
