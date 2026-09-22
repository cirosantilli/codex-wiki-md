<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $E$ record whether the second stage erased the symbol, and write its output as $Z$. The erasure marker is outside the original output alphabet, so $E$ is determined by $Z$. [Independence](../../../../independent-random-variables.md) makes $E$ independent of both $X$ and the first output $Y$. The [chain rule for mutual information](../../../../chain-rule-for-mutual-information.md) therefore gives

$$
I(X;Z)=I(X;E,Z)=I(X;E)+I(X;Z\mid E)
=(1-p)I(X;Y).
$$

The erased branch gives zero information because its output is constant; the unerased branch has exactly the original joint input-output law. Maximizing over the same input distributions gives

$$
\boxed{C_{\rm composite}=(1-p)C}.
$$

This includes $p=0$ and $p=1$. It is the [capacity after independent output erasure](../../../../capacity-after-independent-output-erasure.md); input-dependent erasure would not justify the [independence](../../../../independent-random-variables.md) step.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
