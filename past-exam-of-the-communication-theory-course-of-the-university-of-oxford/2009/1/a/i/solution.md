<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For finite-valued [random vectors](../../../../../random-vector.md), the [conditional entropy](../../../../../conditional-entropy.md) is the average of the entropies of the conditional distributions:

$$
\boxed{H(X\mid Y)=\sum_{y:p_Y(y)>0}p_Y(y)\left[-\sum_xp(x\mid y)\log_2p(x\mid y)\right]}.
$$

Use $0\log_2 0=0$ and omit zero-[probability](../../../../../probability.md) conditioning events. Equivalently,

$$
H(X\mid Y)=-\sum_{x,y:p(x,y)>0}p(x,y)\log_2\frac{p(x,y)}{p_Y(y)}.
$$

The base two makes all information quantities measured in [bits](../../../../../bit.md); changing the logarithm base scales them by a positive constant and preserves the inequalities.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
