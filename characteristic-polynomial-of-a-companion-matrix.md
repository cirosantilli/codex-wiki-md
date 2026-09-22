# Characteristic polynomial of a companion matrix

↑ **Parent:** [Companion matrix](companion-matrix.md)

For a [monic polynomial](monic-polynomial.md) $f(t)=t^d+c_{d-1}t^{d-1}+\cdots+c_0$, use the [companion matrix](companion-matrix.md) convention with ones on the subdiagonal and last column $(-c_0,\ldots,-c_{d-1})^{\mathsf T}$. In $tI-C(f)$, the cofactors of the last-column entries, from top to bottom, are $1,t,\ldots,t^{d-1}$. This follows by expanding their bidiagonal minors: the subdiagonal factors $-1$ cancel the cofactor signs. [Laplace expansion](laplace-expansion.md) along that column therefore gives $c_0+c_1t+\cdots+c_{d-2}t^{d-2}+(t+c_{d-1})t^{d-1}=f(t)$. The degree-one case is the same identity for the one-by-one matrix $(-c_0)$.

## ↑ Ancestors (7)

1. [Companion matrix](companion-matrix.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cyclic operator has equal minimal and characteristic polynomials](cyclic-operator-has-equal-minimal-and-characteristic-polynomials.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2012/1/b/solution.md)
- [Solution](past-exam-of-the-rings-and-modules-course-of-the-university-of-oxford/2017/3/a/solution.md)
