<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $S_N=N^{-3}\sum_{n=1}^N n^2$. The expression in part (ii) gives

$$
T_N=3\left(S_N-\frac1N\right)+\frac3{2N}=3S_N-\frac3{2N}.
$$

Because $3x^2$ is [continuous](../../../../../../continuous-function.md) on $[0,1]$, the [composite trapezoidal rule](../../../../../../composite-trapezoidal-rule.md) converges to its [definite integral](../../../../../../definite-integral.md), which is $1$ by part (i). In fact its standard [composite trapezoidal error bound](../../../../../../composite-trapezoidal-error-bound.md) is $|T_N-1|\leq1/(2N^2)$, since $f''=6$. Therefore

$$
\boxed{\lim_{N\to\infty}S_N=\lim_{N\to\infty}\left(\frac{T_N}{3}+\frac1{2N}\right)=\frac13.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
