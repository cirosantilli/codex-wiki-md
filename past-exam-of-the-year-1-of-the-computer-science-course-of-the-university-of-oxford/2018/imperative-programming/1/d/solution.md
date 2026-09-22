<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Choose the reciprocal-[factorial](../../../../../factorial.md) summation `eb` for asymptotically high accuracy**, counting multiplications and divisions as arithmetic work. For tolerance $\epsilon$, linear powering in part (a)(i) takes $O(\epsilon^{-1})$ multiplications; [binary exponentiation](../../../../../exponentiation-by-squaring.md) in part (a)(ii) reduces this to $O(\log(1/\epsilon))$. Part (c) also has $O(\log(1/\epsilon))$ arithmetic work, since its required $n$ grows like $\epsilon^{-1/2}$, though its constants and [cancellation error](../../../../../cancellation-error.md) differ.

By the [reciprocal-factorial series remainder bound](../../../../../reciprocal-factorial-series-remainder-bound.md), the omitted positive tail satisfies

$$
0<e-e_b(n)=\sum_{j=n+1}^{\infty}\frac1{j!}\leq\frac1{(n+1)!}\sum_{r=0}^{\infty}\frac1{(n+2)^r}=\frac{n+2}{(n+1)(n+1)!}.
$$

Thus the [factorial](../../../../../factorial.md) denominator grows much faster than an exponential in the number of iterations. For $d$ decimal places, setting $\epsilon$ of order $10^{-d}$ gives $n=\Theta(d/\log d)$ by [Stirling's approximation](../../../../../stirling-formula.md), rather than $\Theta(d)$ binary-power arithmetic steps. This is a comparison in an exact-arithmetic operation-count model; the stated [Big O notation](../../../../../big-o-notation.md) does not determine the exact winner for every small tolerance. Taken literally, `eb` uses zero multiplications and only divisions. Fixed [double-precision floating-point format](../../../../../double-precision-floating-point-format.md) cannot deliver arbitrarily many correct decimal places, and the precision-dependent cost of [arbitrary-precision arithmetic](../../../../../arbitrary-precision-arithmetic.md) is a separate issue.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
