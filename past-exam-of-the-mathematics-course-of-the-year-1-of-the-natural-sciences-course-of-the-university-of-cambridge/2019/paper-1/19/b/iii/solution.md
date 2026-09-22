<h1 id="19/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [Exact Newton error identity for a quadratic](../../../../../../exact-newton-error-identity-for-a-quadratic.md) to expose the cancellation without a long quotient expansion. Put $e_k=x_k-x_*$. Since $f(x_*)=0$, direct expansion gives

$$
f(x_k)=2(x_*-\varepsilon)e_k+e_k^2,\qquad
e_{k+1}=e_k-\frac{2(x_*-\varepsilon)e_k+e_k^2}{2(x_*-\varepsilon+e_k)}
=\frac{e_k^2}{2(x_k-\varepsilon)}.
$$

From part (ii), $e_1=\tfrac12\varepsilon^2+O(\varepsilon^3)$ and $x_1-\varepsilon\to1$. It follows that

$$
e_2=\frac{\frac14\varepsilon^4+O(\varepsilon^5)}{2(1+O(\varepsilon^2))}
=\frac18\varepsilon^4+O(\varepsilon^5).
$$

Thus the stronger result is

$$
\boxed{|x_2-x_*|\sim\frac18|\varepsilon|^4,\qquad n_2=4>3.}
$$

The vanishing lower-order terms are a concrete instance of [quadratic convergence](../../../../../../quadratic-convergence.md): to leading order, this step squares the previous error.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [19](../../../19.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
