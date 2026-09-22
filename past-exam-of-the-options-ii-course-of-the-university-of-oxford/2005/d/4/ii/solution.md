<h1 id="d/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose [measurable](../../../../../measurability.md) versions of the two [Lebesgue integrable functions](../../../../../lebesgue-integrable-function.md) and consider $F(x,y)=g(x-y)h(y)$. Translation and the corresponding linear [change of variables](../../../../../change-of-variables-formula.md) preserve Lebesgue measurability; one can first use Borel versions and then disregard the resulting null-set changes. [Tonelli's theorem](../../../../../tonelli-theorem.md) and [translation invariance](../../../../../translation-invariance.md) give

$$
\int_{\mathbb R}\int_{\mathbb R}|g(x-y)h(y)|\,dx\,dy
=\int_{\mathbb R}|h(y)|\,\|g\|_1\,dy
=\|g\|_1\|h\|_1<\infty.
$$

[Fubini theorem](../../../../../fubini-s-theorem.md) therefore shows that the section in $y$ is integrable for [almost every](../../../../../almost-everywhere.md) $x$. Define $(g*h)(x)$ by that section [integral](../../../../../integral-split.md) where it exists and by zero on the exceptional [null set](../../../../../null-set.md). [Fubini theorem](../../../../../fubini-s-theorem.md) also makes this a [measurable](../../../../../measurability.md) [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md), with

$$
\boxed{\|g*h\|_1\le\|g\|_1\|h\|_1.}
$$

Its almost-everywhere defining formula is precisely the desired [convolution](../../../../../convolution.md). This construction explains why an everywhere-existing pointwise [integral](../../../../../integral-split.md) is not required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [D](../../../d.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
