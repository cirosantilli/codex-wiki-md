<h1 id="19/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Leibniz integral rule](../../../../../leibniz-integral-rule.md) accounts for both the moving upper endpoint and the integrand's dependence on $a$:

$$
\boxed{I'(a)=f(a,a)+\int_0^a\frac{\partial f}{\partial a}(x,a)\,dx}.
$$

For the specified integrand this gives $I'(a)=e^{-a^2}-\int_0^ax e^{-ax}\,dx$. When $a\ne0$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_0^ax e^{-ax}\,dx=-e^{-a^2}+\frac{1-e^{-a^2}}{a^2},
$$

so

$$
\boxed{I'(a)=2e^{-a^2}-\frac{1-e^{-a^2}}{a^2}\quad(a\ne0)}.
$$

For the requested independent check, direct integration gives $I(a)=(1-e^{-a^2})/a$ at $a\ne0$. Its [derivative](../../../../../derivative.md) is $[2a^2e^{-a^2}-(1-e^{-a^2})]/a^2$, agreeing with the result above. At zero the apparent singularity is removable: $I(a)=a-a^3/2+O(a^5)$, so $\boxed{I(0)=0,\ I'(0)=1}$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
