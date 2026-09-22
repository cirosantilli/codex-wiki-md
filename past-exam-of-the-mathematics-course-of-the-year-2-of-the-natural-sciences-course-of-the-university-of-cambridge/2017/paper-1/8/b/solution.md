<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert the [Frobenius solution](../../../../../frobenius-solution.md) and its differentiated series into the equation. Collecting the terms before shifting an index gives

$$
\sum_{n=0}^{\infty}(n+\sigma)(n+\sigma+\gamma-1)a_nx^{n+\sigma-1}
-\sum_{n=0}^{\infty}(n+\sigma+\alpha)(n+\sigma+\beta)a_nx^{n+\sigma}=0.
$$

The coefficient of the lowest power $x^{\sigma-1}$ is $a_0\sigma(\sigma+\gamma-1)$. Because $a_0\ne0$, the [indicial equation](../../../../../indicial-equation.md) gives

$$
\boxed{\sigma=0\quad\text{or}\quad\sigma=1-\gamma.}
$$

For the coefficient of $x^{n+\sigma-1}$ with $n\geq1$, shift the index in the second sum. The [hypergeometric Frobenius recurrence](../../../../../hypergeometric-frobenius-recurrence.md) is

$$
\boxed{(n+\sigma)(n+\sigma+\gamma-1)a_n
=(n+\sigma+\alpha-1)(n+\sigma+\beta-1)a_{n-1}.}
$$

Whenever the left coefficient is nonzero, division yields

$$
\boxed{a_n=\frac{(n+\sigma+\alpha-1)(n+\sigma+\beta-1)}{(n+\sigma)(n+\sigma+\gamma-1)}a_{n-1}.}
$$

For noninteger $\gamma$, the two independent local solutions can therefore be identified as

$$
y_1={}_2F_1(\alpha,\beta;\gamma;x),\qquad
y_2=x^{1-\gamma}{}_2F_1(\alpha-\gamma+1,\beta-\gamma+1;2-\gamma;x),
$$

with a consistent local branch for the fractional power. The [hypergeometric function](../../../../../hypergeometric-function.md) coefficients follow by iterating the recurrence using [rising factorials](../../../../../rising-factorial.md).

There is a parameter qualification to the PDF's statement for all real constants: a zero denominator cannot be divided through. At an [undetermined coefficient at Frobenius resonance](../../../../../undetermined-coefficient-at-frobenius-resonance.md), use the undivided coefficient equation to test compatibility. For example, $\gamma=0,\sigma=0,n=1$ requires $0=\alpha\beta a_0$, so a pure exponent-zero series with $a_0\ne0$ is impossible if $\alpha\beta\ne0$. When $\gamma=1$ the two [indicial roots](../../../../../indicial-root.md) coincide, and a second independent solution generally needs a logarithmic term. The [indicial roots](../../../../../indicial-root.md) and undivided relation remain the valid coefficient conclusions in these exceptional cases.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
