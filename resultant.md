# Resultant

↑ **Parent:** [Polynomial](polynomial-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Resultant)

The [resultant](resultant.md) turns a shared-[root of a polynomial](root-of-a-polynomial.md) question into a calculation using only [coefficients](coefficient.md). For nonconstant [univariate polynomials](univariate-polynomial.md) $f,g\in K[x]$ over a [field](field.md) $K$, with their actual [polynomial degrees](degree-of-a-polynomial.md) $m,n$, define

$$
\operatorname{Res}_x(f,g)=\det S(f,g),
$$

where $S(f,g)$ is the [Sylvester matrix](sylvester-matrix.md). Then

$$
\boxed{\operatorname{Res}_x(f,g)=0\quad\Longleftrightarrow\quad f,g\text{ have a common root in }\overline K.}
$$

Here $\overline K$ is an [algebraic closure](algebraic-closure.md). The [common root](common-root.md) need not lie in $K$: two real [polynomials](polynomial-split.md) may share a nonreal [complex root](complex-root.md). The subscript identifies which [variable](variable-mathematics.md) is eliminated.[Algebraic Techniques and Semidefinite Optimization, MIT 6.972, Spring 2006; MIT 6.972, Lecture 6, 28 February 2006, pp. 6-1–6-2, Resultants: Sylvester matrix, root product and common-root criterion](algebraic-techniques-and-semidefinite-optimization-mit-6-972-spring-2006/lecture-6-resultants-and-discriminants.md)

The useful surprise is that a [determinant](determinant.md) detects a shared [root of a polynomial](root-of-a-polynomial.md) without first finding either list of [roots of a polynomial](root-of-a-polynomial.md). If the [coefficients](coefficient.md) depend on a parameter, the [resultant](resultant.md) itself is a [polynomial](polynomial-split.md) in that parameter. Its zeros pick out possible exceptional parameter values. [Elimination theory](elimination-theory.md) uses this to reduce a pair of [polynomial equations](polynomial-equation.md) in two [variables](variable-mathematics.md) to a single necessary equation in one [variable](variable-mathematics.md); [eliminating a variable with a resultant](eliminating-a-variable-with-a-resultant.md) gives an exact example below.

A nonzero [resultant](resultant.md) also supplies a certificate that $f$ and $g$ are [coprime polynomials](coprime-polynomials.md). The [Sylvester matrix](sylvester-matrix.md) then solves for [polynomials](polynomial-split.md) $A,B$ satisfying $Af+Bg=1$, a [Bézout's identity for polynomials](bezout-s-identity-for-polynomials.md). Evaluating such an identity at a hypothetical [common root](common-root.md) would give $0=1$.

**Table of contents**

- [Sylvester matrix](sylvester-matrix.md)
- [Resultant as a product over roots](resultant-as-a-product-over-roots.md)
- [Eliminating a variable with a resultant](eliminating-a-variable-with-a-resultant.md)
  - [Degree drop in a specialized resultant](degree-drop-in-a-specialized-resultant.md)

## ↑ Ancestors (5)

1. [Polynomial](polynomial-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Degree drop in a specialized resultant](degree-drop-in-a-specialized-resultant.md)
- [Eliminating a variable with a resultant](eliminating-a-variable-with-a-resultant.md)
- [Elimination theory](elimination-theory.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-14/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/18h/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-32/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-125/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-125/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/18g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-125/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-125/3/a/solution.md)
- [Resultant](resultant.md)
- [Resultant as a product over roots](resultant-as-a-product-over-roots.md)
- [Resultant bound for intersections of plane curves](resultant-bound-for-intersections-of-plane-curves.md)
- [Squarefree reduction excludes a prime from the power-basis index](squarefree-reduction-excludes-a-prime-from-the-power-basis-index.md)
- [Sylvester matrix](sylvester-matrix.md)
