<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the target [probability density function](../../../../../../../probability-density-function.md) is supported where the proposal [probability density function](../../../../../../../probability-density-function.md) is positive and that the envelope constant is finite. Any $C\ge M$ satisfies $f(x)\le Cg(x)$, and integration gives $C\ge1$. For each attempt draw independently $Y\sim g$ and $U\sim U(0,1)$. **Accept $Y$ if $U\le f(Y)/(Cg(Y))$; otherwise discard it and repeat.** Independent attempts give independent accepted values. A finite pre-generated list of independent proposal draws can be screened with independent uniforms in the same way, though the number retained is random. If $M=\infty$, this fixed-envelope [rejection sampling](../../../../../../../rejection-sampling.md) method cannot be used with that proposal.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
