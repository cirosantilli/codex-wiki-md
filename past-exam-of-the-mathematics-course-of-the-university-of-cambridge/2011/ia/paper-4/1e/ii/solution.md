<h1 id="1e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Can be false.** Take $X=\{0,1,2,\ldots\}$ and define

$$
g(n)=n+1,\qquad f(0)=0,\qquad f(n)=n-1\quad(n\geq1).
$$

Then $(f\circ g)(n)=n$, so their [function composition](../../../../../../function-composition.md) is the [identity function](../../../../../../identity-function.md) and hence a [bijection](../../../../../../bijection.md). However, $g$ is not [surjective](../../../../../../surjective-function.md), since zero has no preimage, while $f$ is not [injective](../../../../../../injective-function.md), since $f(0)=f(1)=0$.

The valid implications are only that $g$ must be [injective](../../../../../../injective-function.md) and $f$ must be [surjective](../../../../../../surjective-function.md): equality of two $g$ values implies equality after composition, and every output of the composition is an output of $f$. On a finite $X$, either of these properties implies a [bijection](../../../../../../bijection.md), so an infinite set is essential to this counterexample.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1E](../../1e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
