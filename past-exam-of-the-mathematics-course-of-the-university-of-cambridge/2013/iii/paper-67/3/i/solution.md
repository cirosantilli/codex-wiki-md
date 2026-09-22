<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Reversing the drift reverses the endpoint carrying the [boundary layer](../../../../../../boundary-layer.md). The outer equation is $-(1+x)^2y_0'+y_0=0$, and now its condition comes from $x=0$:

$$
y_0(x)=e^{1-1/(1+x)}.
$$

Its value at $x=1$ is $e^{1/2}$, so it cannot by itself satisfy the right boundary value. Put $\xi=(1-x)/\epsilon$ there. The leading inner equation is $Y''+4Y'=0$, with a correction proportional to $e^{-4\xi}$ that decays into the domain. Thus **the outer region has size $O(1)$ and the right endpoint layer has width $O(\epsilon/4)=O(\epsilon)$**. One would expand the coefficient near $x=1$, solve the successive equations for the [inner expansion](../../../../../../inner-expansion.md), match as $\xi\to\infty$, and form a [matched asymptotic expansion](../../../../../../matched-asymptotic-expansion.md) by subtracting the overlap. No turning region occurs because the drift does not vanish on this interval.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
