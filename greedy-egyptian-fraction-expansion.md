# Greedy Egyptian fraction expansion

↑ **Parent:** [Egyptian fraction](egyptian-fraction.md)

For a positive proper residual [fraction](fraction.md) $n/d$, with $0<n<d$, choose $q=\lceil d/n\rceil$, append the [unit fraction](unit-fraction.md) $1/q$, and replace the residual by $(nq-d)/(dq)$ in lowest terms. This is a [greedy algorithm](greedy-algorithm.md): the chosen [unit fraction](unit-fraction.md) is the largest one not exceeding the residual.

The inequalities $q-1<d/n\leq q$ imply $0\leq nq-d<n$. Thus the numerator of the reduced residual strictly decreases while positive, proving [algorithm termination](algorithm-termination.md) by a nonnegative-[integer](integer-split.md) [loop variant](loop-variant.md). The [loop invariant](loop-invariant.md) is that the accumulated [sum](sum.md) plus the residual is the original [rational number](rational-number.md). Since $q\geq2$ and $n/d<1/(q-1)$, the new residual is less than $1/(q(q-1))\leq1/q$. If it remains positive, its next chosen denominator is therefore strictly greater than $q$; this expansion also satisfies the distinct-denominator convention. The proof does not bound the denominators by the input's fixed-width range. [Arbitrary-precision arithmetic](arbitrary-precision-arithmetic.md), checked conversion, or a different representable expansion can therefore be necessary in code.

## ↑ Ancestors (8)

1. [Egyptian fraction](egyptian-fraction.md)
2. [Unit fraction](unit-fraction.md)
3. [Fraction](fraction.md)
4. [Rational number](rational-number.md)
5. [Number theory](number-theory-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/4/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/1/c/solution.md)
