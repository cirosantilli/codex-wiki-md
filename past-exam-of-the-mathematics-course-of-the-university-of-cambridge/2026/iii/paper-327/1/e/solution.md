<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Although $|u(x)|=e^{x^2}$ has superpolynomial growth, the rapidly varying phase makes $u$ an [oscillatory](../../../../../../oscillatory-integral.md) tempered distribution. Split the integral against $\varphi\in\mathcal S(\mathbb R)$ into $|x|\leq1$ and the two tails. On a tail, with $\Phi(x)=e^{x^4}$,

$$
e^{i\Phi(x)}=\frac1{i\Phi'(x)}\frac d{dx}e^{i\Phi(x)},\qquad\Phi'(x)=4x^3e^{x^4}.
$$

Integration by parts transfers the derivative to

$$
\frac{e^{x^2}\varphi(x)}{4x^3e^{x^4}}.
$$

This function and its derivative are integrable because $e^{x^2-x^4}$ dominates every polynomial, and the boundary term at infinity vanishes. The result is bounded by finitely many [Schwartz space](../../../../../../schwartz-space.md) seminorms. The compact part has the same property. Thus the cutoff integrals converge and define a continuous linear functional:

$$
\boxed{u\in\mathcal S'(\mathbb R)}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
