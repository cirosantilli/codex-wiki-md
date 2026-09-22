<h1 id="8/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $0\leq s\leq1$, condition on $N=n$. Its [independence](../../../../../../independent-random-variables.md) from the $X_i$ preserves their independent common [distribution](../../../../../../distribution-mathematical-analysis.md), so part (ii) gives

$$
\mathbb E[s^Y\mid N=n]=[G_X(s)]^n.
$$

For $n=0$, this is $1$, agreeing with $Y=0$. By the [law of total expectation](../../../../../../law-of-total-expectation.md),

$$
G_Y(s)=\sum_{n=0}^{\infty}\mathbb P(N=n)[G_X(s)]^n
=\boxed{G_N(G_X(s))}.
$$

This proves the [probability generating function of an independent random sum](../../../../../../probability-generating-function-of-an-independent-random-sum.md). For nonnegative $s$ outside $[0,1]$, the same argument is valid whenever the right side is finite, by [Tonelli's theorem](../../../../../../tonelli-theorem.md) for nonnegative sums. For signed or complex $s$, a sufficient absolute-convergence condition is $G_N(G_X(|s|))<\infty$; it holds automatically on $|s|\leq1$. Outside this domain, mere evaluation of an analytically extended expression is not a substitute for existence of the [probability generating function](../../../../../../probability-generating-function.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
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
