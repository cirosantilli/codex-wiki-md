<h1 id="17d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Integrate the two exponentials in $\cos(\alpha x)$ against $e^{-inx}$. For $\alpha\notin\mathbb Z$ there are no zero denominators, and

$$
 c_n=\frac1{2\pi}\left[\frac{\sin\pi(\alpha-n)}{\alpha-n}
 +\frac{\sin\pi(\alpha+n)}{\alpha+n}\right]
 =\boxed{\frac{(-1)^n\alpha\sin(\pi\alpha)}{\pi(\alpha^2-n^2)}}.
$$

Thus the [complex Fourier series](../../../../../../complex-fourier-series.md) is

$$
 \boxed{\cos(\alpha x)=\frac{\alpha\sin(\pi\alpha)}\pi
 \sum_{n\in\mathbb Z}\frac{(-1)^ne^{inx}}{\alpha^2-n^2},\qquad -\pi\leq x\leq\pi.}
$$

This is the periodic extension, not a globally nonperiodic cosine formula. For each fixed complex $\alpha$, the coefficients are $O(n^{-2})$, giving absolute and uniform convergence. The extension is continuous at the endpoints because the two endpoint values agree; piecewise smooth [pointwise convergence of a piecewise smooth Fourier series](../../../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md) identifies the sum with it, including those endpoints.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [17D](../../17d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
