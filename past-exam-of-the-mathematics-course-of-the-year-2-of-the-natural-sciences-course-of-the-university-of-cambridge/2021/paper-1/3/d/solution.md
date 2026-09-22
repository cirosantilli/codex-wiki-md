<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Insert the source into the [Green-function representation](../../../../../green-function-representation.md) and split the integral at its source discontinuity in [derivative](../../../../../derivative.md):

$$
\begin{aligned}
y(x)&=-e^x\cos x\int_0^x\sin\xi\,d\xi-e^x\sin x\int_x^{\pi/2}\cos\xi\,d\xi\\
&=-e^x[\cos x(1-\cos x)+\sin x(1-\sin x)].
\end{aligned}
$$

Using $\sin^2x+\cos^2x=1$, the answer is

$$
\boxed{y(x)=e^x(1-\cos x-\sin x).}
$$

Both endpoint values are zero. As a direct check, conjugating by $e^x$ sends $y''-2y'+2y$ to $e^x(v''+v)$, and $v=1-\cos x-\sin x$ gives $v''+v=1$. Thus the differential equation and both [boundary conditions](../../../../../boundary-condition.md) are satisfied.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
