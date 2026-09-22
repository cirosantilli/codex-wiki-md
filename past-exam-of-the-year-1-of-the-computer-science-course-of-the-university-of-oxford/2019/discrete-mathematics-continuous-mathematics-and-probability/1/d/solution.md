<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The [iterated function](../../../../../iterated-function.md) is $f^{(n)}(x)=\sqrt{x^2+n}$ for every positive integer $n$.** The exponent here denotes repeated [function composition](../../../../../function-composition.md), not an ordinary power or a [derivative](../../../../../derivative.md).

For the base case $n=1$, the formula is the definition. If it holds at $n$, then

$$
f^{(n+1)}(x)=f(f^{(n)}(x))
=\sqrt{\left(\sqrt{x^2+n}\right)^2+1}
=\sqrt{x^2+n+1}.
$$

This proves the claim by [mathematical induction](../../../../../mathematical-induction.md), for every real input $x$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
