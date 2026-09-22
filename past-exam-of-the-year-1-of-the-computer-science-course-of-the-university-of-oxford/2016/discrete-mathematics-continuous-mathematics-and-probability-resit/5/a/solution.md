<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Divide $[a,b]$ into $N$ equal subintervals of width $h=(b-a)/N$, with $x_j=a+jh$. Linear interpolation between adjacent values of $f$ gives a trapezoid of signed area $h(f(x_{j-1})+f(x_j))/2$. Adding these areas produces the [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md)

$$
\boxed{T_N=h\left(\frac{f(a)+f(b)}2+\sum_{j=1}^{N-1}f(x_j)\right)\approx\int_a^bf(x)\,dx}.
$$

For continuous $f$, this tends to the [integral](../../../../../integral-split.md) as $h\to0$; if $f$ has a bounded continuous second [derivative](../../../../../derivative.md), the error is at most $(b-a)h^2\max|f''|/12$.

The original PDF prints $n\to\infty$ while using $n$ as the bound summation index and $N$ as the upper limit. Literally this does not specify a varying upper limit. Interpreting the intended limit as **$N\to\infty$**, and relabelling the summation index $j$, gives the [right Riemann sum](../../../../../right-riemann-sum.md)

$$
S_N=\frac1N\sum_{j=1}^N\left(\frac jN\right)^4=\frac1{N^5}\sum_{j=1}^Nj^4.
$$

For $f(x)=x^4$, $a=0$, and $b=1$, the only difference from the [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md) is the endpoint weighting: $S_N=T_N+1/(2N)$. Hence

$$
\boxed{\lim_{N\to\infty}\frac1{N^5}\sum_{j=1}^Nj^4=\int_0^1x^4\,dx=\frac15}.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
