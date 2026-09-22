<h1 id="b/7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Compute $C$ from part (b), solve the [finite element](../../../../../finite-element.md) equations, and calculate the element indicators $\eta_i^2=h_i^4\|R_h\|_{L^2(I_i)}^2$. Let $\eta=(\sum_i\eta_i^2)^{1/2}$. **Stop when $C\eta<\mathrm{TOL}$**; the proved reliability bound then certifies the requested true-error tolerance.

Otherwise mark elements carrying a chosen fraction of the total indicator, bisect them, and repeat. To ensure termination as well as a valid stopping test, include a uniform-refinement safeguard, for example bisect every element on every second unsuccessful pass. This preserves adaptive refinement on the other passes while forcing $h_{\max}\to0$.

Here termination can be justified directly. On each element $R_h=f+p'u_h'-qu_h$, so its global $L^2$ [norm](../../../../../norm.md) stays bounded if $\|u_h\|_{H^1}$ stays bounded. That stability follows from [coercivity](../../../../../coercive-function.md) after subtracting the fixed lift one at the right endpoint. Hence

$$
\eta\leq h_{\max}^2\|R_h\|_{L^2}\longrightarrow0.
$$

The safeguarded algorithm therefore eventually satisfies the strict tolerance. Reliable numerical evaluation of the residual integrals, or an upper bound for their quadrature errors, is part of using the certificate in an implementation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
