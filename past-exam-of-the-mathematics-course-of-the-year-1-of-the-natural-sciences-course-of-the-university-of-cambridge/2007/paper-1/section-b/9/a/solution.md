<h1 id="section-b/9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x\in(n,n+1)$, strict decrease gives $f(x)<f(n)$, while for $x\in(n-1,n)$ it gives $f(x)>f(n)$. Integrating over these unit intervals proves

$$
S_n=\int_n^{n+1}f(x)\,dx<f(n)<\int_{n-1}^nf(x)\,dx=S_{n-1}.
$$

Summing the rectangle bounds gives

$$
\int_2^{M+1}f(x)\,dx<\sum_{n=2}^Mf(n)<f(2)+\int_2^Mf(x)\,dx.
$$

The [partial sums](../../../../../../partial-sum.md) and the [improper integral](../../../../../../improper-integral.md) are nondecreasing. These bounds show that one is bounded exactly when the other is bounded, proving the [integral test for convergence](../../../../../../integral-test-for-convergence.md). In the convergent case, sum the same interval inequalities for $n=N+1,N+2,\ldots$ to obtain

$$
\int_{N+1}^\infty f(x)\,dx<R_N:=\sum_{n=N+1}^\infty f(n)<\int_N^\infty f(x)\,dx.
$$

For $f(x)=1/(x\ln x)$, the [antiderivative](../../../../../../antiderivative.md) is $\ln(\ln x)$, which grows without bound, so the first [series](../../../../../../series-mathematics.md) **diverges**. For $f(x)=1/[x(\ln x)^2]$, the [antiderivative](../../../../../../antiderivative.md) is $-1/\ln x$, whose tail [integral](../../../../../../integral-split.md) is finite, so the second [series](../../../../../../series-mathematics.md) **converges**, with

$$
\boxed{\frac1{\ln(N+1)}<R_N<\frac1{\ln N},\qquad N\geq2.}
$$

Both [functions](../../../../../../function-split.md) are positive and strictly decreasing on $[2,\infty)$, as required.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [9](../../9.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
