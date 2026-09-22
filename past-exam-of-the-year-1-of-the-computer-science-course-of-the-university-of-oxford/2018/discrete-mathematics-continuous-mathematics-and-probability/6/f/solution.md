<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For $n$ equal strips and a uniform bound $|f''(x)|\leq M$ on $[a,b]$, the [composite trapezoidal error bound](../../../../../composite-trapezoidal-error-bound.md) is

$$
|I-T_n|\leq\frac{(b-a)^3M}{12n^2}.
$$

On $[1,25]$, part (b) gives $M=1/2$: $f''$ is positive and decreases from $1/2$ after $x=1$. Hence

$$
|I-T_n|\leq\frac{24^3}{24n^2}=\frac{576}{n^2}.
$$

To certify error at most $10^{-4}$, choose **$n\geq2400$**; equality gives exactly $10^{-4}$ in this bound. This is a sufficient certificate, not a claim that every smaller $n$ fails in actual numerical error.

Strictly, the maximum specified over the open interval $(1,25)$ is not attained; its [supremum](../../../../../supremum.md) is $1/2$. Using the maximum on the closed interval, or simply the uniform bound $M=1/2$, gives the valid error estimate above.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
