<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are

$$
\rho(\zeta)=\zeta^2-(1+a)\zeta+a=(\zeta-1)(\zeta-a),\qquad
\sigma(\zeta)=\frac{1-3a}{2}\zeta+\frac{1+a}{2}\zeta^2.
$$

To determine formal order, substitute a smooth exact solution and expand about the first time level. The [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md) collects precisely the same coefficients:

$$
\rho(e^z)-z\sigma(e^z)
=-\frac{1+5a}{12}z^3-\frac{3+11a}{24}z^4+O(z^5).
$$

The constant, linear and quadratic coefficients vanish for every $a$. The cubic coefficient vanishes only at $a=-1/5$, where the quartic coefficient is $-1/30\ne0$. Hence

$$
\boxed{p=3\text{ if }a=-\tfrac15,\qquad p=2\text{ otherwise}.}
$$

Here order means the exact-solution step residual is $O(h^{p+1})$. It is a formal consistency result, not a convergence assertion. In particular at $a=1$ both $\rho'(1)$ and $\sigma(1)$ vanish, and the double root at one destroys [zero-stability](../../../../../../zero-stability.md); cancelling its common factor gives a different, first-order recurrence with an additional integration constant left unspecified by the original formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
