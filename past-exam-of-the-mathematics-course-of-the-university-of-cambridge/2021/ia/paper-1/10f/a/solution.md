<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Pointwise on $[a,b]$,

$$
mg(x)\leq f(x)g(x)\leq Mg(x)
$$

because $g(x)>0$. To see the implication directly from the definition, every Riemann sum of the nonnegative continuous function $(f-m)g$ is nonnegative, so its limit is nonnegative:

$$
\int_a^b(f-m)g\geq0.
$$

Applying the same argument to $(M-f)g$ gives $\int_a^b(M-f)g\geq0$. By linearity, these are exactly the [monotonicity of the Riemann integral](../../../../../../monotonicity-of-the-riemann-integral.md) bounds

$$
\boxed{
m\int_a^bg(x)\,dx
\leq\int_a^bf(x)g(x)\,dx
\leq M\int_a^bg(x)\,dx}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
