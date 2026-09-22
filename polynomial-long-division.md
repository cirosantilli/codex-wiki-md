# Polynomial long division

↑ **Parent:** [Polynomial division](polynomial-division.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_long_division)

Start with a provisional [polynomial quotient](quotient-of-polynomial-division.md) $q=0$ and remainder $h=f$. If $h$ has [polynomial degree](degree-of-a-polynomial.md) $n$ at least the divisor's [polynomial degree](degree-of-a-polynomial.md) $m$, with [leading coefficients](leading-coefficient-of-a-polynomial.md) $a$ and $b$, subtract $t g$, where

$$
t=\frac{a}{b}X^{n-m},\qquad q\longleftarrow q+t,\qquad h\longleftarrow h-tg.
$$

The identity $f=gq+h$ survives each step, while the leading term cancels and the [polynomial degree](degree-of-a-polynomial.md) of nonzero $h$ strictly decreases. Stop when $h=0$ or $\deg h<m$.

For uniqueness over a [field](field.md), subtract two proposed decompositions:

$$
g(q_1-q_2)=r_2-r_1.
$$

If $q_1\ne q_2$, the left side has [polynomial degree](degree-of-a-polynomial.md) at least $\deg g$, while the right side is zero or has smaller [polynomial degree](degree-of-a-polynomial.md). Hence $q_1=q_2$ and then $r_1=r_2$.[Abstract Algebra, Chapter 3 Ring theory, §3.9, Theorem 3.9.1 and proof: cancellation, termination and degree comparison for uniqueness](abstract-algebra-by-romyar-sharifi/chapter-3-ring-theory.md)

## ↑ Ancestors (6)

1. [Polynomial division](polynomial-division.md)
2. [Polynomial](polynomial-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computer-networks/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-iv/7/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/3/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/4/d/solution.md)
- [Polynomial division](polynomial-division.md)
