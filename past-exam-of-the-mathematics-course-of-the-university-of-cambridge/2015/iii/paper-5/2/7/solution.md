<h1 id="2/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

If unit vectors $f_n$ satisfy $(L-\lambda I)f_n\to0$, a bounded inverse would give $1\le\|(L-\lambda I)^{-1}\|\|(L-\lambda I)f_n\|\to0$. Hence $\lambda$ belongs to the [spectrum of a bounded operator](../../../../../../spectrum-of-a-bounded-operator.md).

Conversely a spectral point is real by the preceding argument. Put $A=L-\lambda I$, again a [self-adjoint operator](../../../../../../self-adjoint-operator.md). If $\inf_{\|f\|=1}\|Af\|>0$, then $A$ is injective with closed range. Its range is dense by [image-kernel orthogonality for an adjoint](../../../../../../image-kernel-orthogonality-for-an-adjoint.md), so it is bijective with a bounded inverse, a contradiction. Thus this infimum is zero; choose unit $f_n$ with $\|Af_n\|<1/n$. We have proved

$$
\boxed{\lambda\in\Sigma(L)\iff\exists(f_n):\ \|f_n\|=1,\quad(L-\lambda I)f_n\to0.}
$$

Such a sequence is a [spectral Weyl sequence](../../../../../../spectral-weyl-sequence.md). No weak convergence is required here; nonreal $\lambda$ are ruled out by the lower bound in the preceding solution.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
