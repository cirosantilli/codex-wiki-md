# Euclidean algorithm

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_algorithm)

For positive [integers](integer.md) $a,b$, the Euclidean algorithm repeatedly performs [division with remainder](euclidean-division.md): write $a=qb+r$ with $0\leq r<b$, then replace $(a,b)$ by $(b,r)$ until the second entry is zero. The final nonzero entry is their [greatest common divisor](greatest-common-divisor.md). A remainder preserves the set of common [divisors](divisor.md): an [integer](integer.md) divides $a$ and $b$ exactly when it divides $b$ and $a-qb$. The positive remainders strictly decrease, so the calculation terminates.

The complete calculation for $252$ and $198$ is

$$
\begin{aligned}
252&=1\cdot198+54,\\
198&=3\cdot54+36,\\
54&=1\cdot36+18,\\
36&=2\cdot18+0.
\end{aligned}
$$

Hence **$\gcd(252,198)=18$**. The [fraction](fraction.md) $252/198$ reduces to $14/11$ by dividing numerator and denominator by that common factor. The same remainder calculation has a geometric interpretation: remove squares from a $252$-by-$198$ [rectangle](rectangle.md), then repeat on the remaining strip. Each division step records how many equal squares fit and the width of the new strip.

<a id="image-successive-square-removals-record-the-euclidean-algorithm-for-252-and-198"></a>
![](euclidean-algorithm-rectangles.png)

**[Figure 46](#image-successive-square-removals-record-the-euclidean-algorithm-for-252-and-198). Successive square removals record the Euclidean algorithm for 252 and 198**.

The procedure does more than test individual [divisors](divisor.md). Each step replaces the whole common-divisor problem by a smaller equivalent one. Euclid's Book VII, Proposition 2 describes the corresponding repeated-subtraction construction; batching those subtractions into [division with remainder](euclidean-division.md) gives the present formulation. [Euclid, Elements VII.2, greatest common measure](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII2.html)

**Table of contents**

- [Extended Euclidean algorithm](extended-euclidean-algorithm.md)
- [Linear Diophantine equation](linear-diophantine-equation.md)
  - [All solutions of a linear Diophantine equation](all-solutions-of-a-linear-diophantine-equation.md)
  - [Linear Diophantine equation solvability criterion](linear-diophantine-equation-solvability-criterion.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Computing Legendre symbols by quadratic reciprocity](computing-legendre-symbols-by-quadratic-reciprocity.md)
- [Divisibility](divisibility.md)
- [Extended Euclidean algorithm](extended-euclidean-algorithm.md)
- [Fibonacci gcd reduction](fibonacci-gcd-reduction.md)
- [Greatest common divisor](greatest-common-divisor.md)
- [Integer factorization](integer-factorization.md)
- [Least common multiple](least-common-multiple.md)
- [Linear congruence](linear-congruence.md)
- [Lucas number](lucas-number.md)
- [Number theory](number-theory-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-20/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/1e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/12j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-4/1e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-17/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-24/5/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-29/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/4h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-27/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-27/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/1d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/11e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/6e/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/1g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/1g/ii/solution.md)
- [Quotient by an irreducible polynomial is a field](quotient-by-an-irreducible-polynomial-is-a-field.md)
