<h1 id="14/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $n$ independent seeds the [probability](../../../../../probability.md) of at least one success is $1-(1-x)^n$. Requiring it to be at least $0.95$ gives $(1-x)^n\leq0.05$. For $0<x<1$, taking logarithms and dividing by the negative number $\log(1-x)$ reverses the inequality:

$$
n\geq\frac{\log0.05}{\log(1-x)}.
$$

The smallest permitted integer is therefore

$$
\boxed{n_{\min}=\left\lceil\frac{\log0.05}{\log(1-x)}\right\rceil}.
$$

The [ceiling function](../../../../../ceiling-function.md) is necessary because seeds are counted discretely. If $x=0$, no finite number suffices; if $x=1$, one seed suffices. The target is interpreted as at least a ninety-five percent chance, since exact equality may not be attainable with an integer count.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [14](../../14.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
