<h1 id="f/f2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Differentiability](../../../../../differentiability.md) at $x_0$ means that a [linear map](../../../../../linear-map.md) $L:\mathbb R^n\to\mathbb R^m$ exists such that $f(x_0+h)=f(x_0)+Lh+o(\|h\|)$. Since finite-dimensional [linear maps](../../../../../linear-map.md) are [bounded](../../../../../boundedness.md), the right side tends to $f(x_0)$ as $h\to0$, proving [continuity](../../../../../continuous-function.md).

For the specified scalar function, $0\le f(x,y)\le x^2\le x^2+y^2$. Dividing by $\sqrt{x^2+y^2}$ gives a bound tending to zero at the origin. Consequently $\boxed{df(0,0)=0}$ and the function is [differentiable](../../../../../differentiable-function.md) there.

For the final product assertion, write $f(x_0+h)=Lh+r(h)$, where $r(h)=o(\|h\|)$, and $g(x_0+h)=g(x_0)+s(h)$ with $s(h)=o(1)$. Since $f(x_0)=0$,

$$
F(x_0+h)-F(x_0)-\langle Lh,g(x_0)\rangle=\langle Lh,s(h)\rangle+\langle r(h),g(x_0)+s(h)\rangle=o(\|h\|).
$$

[Cauchy](../../../../../cauchy-sequence.md)–Schwarz and [boundedness](../../../../../boundedness.md) of $g$ near $x_0$ justify the last estimate. Thus $\boxed{dF(x_0)h=\langle df(x_0)h,g(x_0)\rangle}$; [differentiability](../../../../../differentiability.md) of $g$ is unnecessary because $f(x_0)=0$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
