<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the principal [complex logarithm](../../../../../../complex-logarithm.md) in the upper half-plane. Deform the interval upward into a half-strip: the vertical side at zero is traversed upward, and the side at one downward. The top side vanishes exponentially; a small indentation at zero contributes $O(r|\log r|)$ and vanishes. Thus the [contour deformation](../../../../../../contour-deformation.md) gives the exact representation, for $x>0$,

$$
f(x)=i\int_0^\infty\log(is)e^{-xs}\,ds
-i e^{ix}\int_0^\infty\log(1+is)e^{-xs}\,ds.
$$

Since $\log(is)=\log s+i\pi/2$, scaling $u=xs$ and using the integral defining [Euler's constant](../../../../../../euler-s-constant.md) gives

$$
i\int_0^\infty\log(is)e^{-xs}\,ds
=-\frac{i(\log x+\gamma)}x-\frac\pi{2x}.
$$

For the second endpoint, $\log(1+is)=is+s^2/2+O(s^3)$. [Watson's lemma](../../../../../../watson-s-lemma.md), or integration of these powers against $e^{-xs}$ with an exponentially small tail, yields

$$
-i e^{ix}\int_0^\infty\log(1+is)e^{-xs}\,ds
=\frac{e^{ix}}{x^2}-\frac{i e^{ix}}{x^3}+O(x^{-4}).
$$

In particular **the required first terms are**

$$
\boxed{f(x)=-\frac{i\log x}{x}-\frac{i\gamma+\pi/2}{x}
+\frac{e^{ix}}{x^2}+O(x^{-3}).}
$$

The two different endpoint scales come from the [logarithmic singularity](../../../../../../logarithmic-singularity.md) at zero and the simple zero of the amplitude at one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
