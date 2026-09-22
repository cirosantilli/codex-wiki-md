<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $t=0$, the [initial conditions](../../../../../initial-condition.md) imply

$$
f(x)+g(x)=u(x),\qquad c\bigl(f'(x)-g'(x)\bigr)=v(x).
$$

Differentiate the first relation and solve for the two [derivatives](../../../../../derivative.md):

$$
f'=\frac12u'+\frac1{2c}v,\qquad
g'=\frac12u'-\frac1{2c}v.
$$

Fix a reference point $x_*$ and set $V(x)=\int_{x_*}^xv(s)\,ds$. Taking [antiderivatives](../../../../../antiderivative.md) gives

$$
\boxed{f(x)=\frac12u(x)+\frac1{2c}V(x)+K,\qquad
g(x)=\frac12u(x)-\frac1{2c}V(x)-K}.
$$

The constants must be opposite to preserve the first [initial condition](../../../../../initial-condition.md); the arbitrary [constant of integration](../../../../../constant-of-integration.md) $K$ does not change $\psi$. Substitution yields [D'Alembert's formula](../../../../../d-alembert-s-formula.md):

$$
\boxed{\psi(x,t)=\frac{u(x+ct)+u(x-ct)}2
+\frac1{2c}\int_{x-ct}^{x+ct}v(s)\,ds}.
$$

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) verifies that its time [derivative](../../../../../derivative.md) at zero is $v(x)$, and its value at zero is $u(x)$. The oriented [integral](../../../../../integral-split.md) also makes the formula valid for negative $t$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
