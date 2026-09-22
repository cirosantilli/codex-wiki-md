<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $B=|b|>0$. For $a>0$, integrate $e^{iaz}/(z^2+B^2)$ over the upper semicircle. [Jordan's lemma](../../../../../jordan-s-lemma.md) removes the arc, and the [residue theorem](../../../../../residue-theorem.md) at $z=iB$ gives

$$
\int_{-\infty}^{\infty}\frac{e^{iax}}{x^2+B^2}\,dx
=2\pi i\frac{e^{-aB}}{2iB}=\frac\pi B e^{-aB}.
$$

Taking the real part and using [evenness](../../../../../even-function.md) in both $x$ and $a$ yields

$$
\boxed{I_1(a)=\frac{\pi}{2B}e^{-B|a|}.}
$$

The case $a=0$ follows directly from an [inverse tangent](../../../../../inverse-tangent.md) primitive. The complex exponential is essential on the contour: the cosine alone has a growing exponential component.

For $a>0$, [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) gives $-I_1'(a)=\int_0^\infty x\sin(ax)/(x^2+B^2)\,dx$. This derivative is a conditionally convergent [improper integral](../../../../../improper-integral.md); the [Dirichlet test](../../../../../dirichlet-test.md) makes its tails uniform on compact subintervals of $a>0$, justifying the differentiation. Setting $a=1$ gives

$$
\boxed{I_2=\frac\pi2e^{-B}.}
$$

Finally let $J(a)=\int_0^\infty\sin(ax)/[x(x^2+B^2)]\,dx$. Its differentiated integrand is absolutely integrable, so $J'(a)=I_1(a)$ and $J(0)=0$. Hence

$$
\boxed{I_3=J(1)=\frac{\pi}{2B^2}(1-e^{-B}).}
$$

If $b=0$, $I_1$ and $I_3$ diverge at the origin, whereas $I_2=\int_0^\infty\sin x/x\,dx=\pi/2$ is the corresponding [Dirichlet integral](../../../../../dirichlet-integral.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
