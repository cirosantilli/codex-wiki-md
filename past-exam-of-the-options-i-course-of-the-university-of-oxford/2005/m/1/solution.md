<h1 id="m/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [moment-generating function](../../../../moment-generating-function.md) is $M_X(t)=\mathbb E[e^{tX}]$ where finite. For [independent](../../../../independent-random-variables.md) $X,Y$, [independence](../../../../independent-random-variables.md) factors the expectation, giving $M_{X+Y}(t)=M_X(t)M_Y(t)$ wherever both factors are finite.

For the given [probability density function](../../../../probability-density-function.md) and $t<1$, put $s=(1-t)x$ to obtain

$$
M_{X_n}(t)=\frac1{(n-1)!}\int_0^\infty x^{n-1}e^{-(1-t)x}\,dx=\frac{\Gamma(n)}{(n-1)!(1-t)^n}=\boxed{(1-t)^{-n}}.
$$

Here $\Gamma(n)=(n-1)!$, obtained by repeated [integration by parts](../../../../integration-by-parts.md). For $t\geq1$ the defining integral diverges.

Each $Y_i$ has [moment-generating function](../../../../moment-generating-function.md) $(1-t)^{-1}$, so [independence](../../../../independent-random-variables.md) gives

$$
M_{\sum_{i=1}^nY_i}(t)=(1-t)^{-n}\quad(t<1).
$$

The [uniqueness theorem for moment-generating functions](../../../../uniqueness-theorem-for-moment-generating-functions.md) applies when the functions are finite on a [neighborhood](../../../../neighbourhood-mathematics.md) of zero. Hence **the sum has the same distribution as $X_n$**, a [Gamma distribution](../../../../gamma-distribution.md) of shape $n$ and rate one, with the displayed [probability density function](../../../../probability-density-function.md) in the source.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [M](../../m.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
