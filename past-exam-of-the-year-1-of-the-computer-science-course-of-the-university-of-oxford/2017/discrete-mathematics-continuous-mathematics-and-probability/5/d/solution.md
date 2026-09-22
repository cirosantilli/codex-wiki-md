<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $h=1/N$, the [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md) is

$$
T_N(f)=\frac1N\left(\frac{f(0)}2+\sum_{m=1}^{N-1}f(m/N)+\frac{f(1)}2\right).
$$

With $f(x)=1/(4-x^2)$ this becomes

$$
T_N=\frac{7}{24N}+\sum_{m=1}^{N-1}\frac{N}{4N^2-m^2}.
$$

Write the requested right [Riemann sum](../../../../../riemann-sum.md) as $S_N$. The [trapezoidal endpoint correction for a right Riemann sum](../../../../../trapezoidal-endpoint-correction-for-a-right-riemann-sum.md) gives

$$
S_N-T_N=\frac{f(1)-f(0)}{2N}=\frac1{24N}.
$$

The integrand is continuous on $[0,1]$, so the trapezoidal values converge to its definite integral; the endpoint correction tends to zero. Therefore

$$
\boxed{\lim_{N\to\infty}\sum_{m=1}^N\frac{N}{4N^2-m^2}=\frac14\log3.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
