<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

Because $x^*$ is an interior minimizer of the differentiable function $f$, it satisfies $f'(x^*)=0$. Apply the [Taylor theorem with Lagrange remainder](../../../../../taylor-theorem-with-lagrange-remainder.md) to $f'$ about $x_n$. For some $y_n$ between $x_n$ and $x^*$,

$$
0=f'(x^*)
=f'(x_n)+f''(x_n)(x^*-x_n)
+\frac12f'''(y_n)(x^*-x_n)^2.
$$

The lower bound on $|f''|$ ensures that every step of the [Newton method](../../../../../newton-s-method-in-optimization.md) is defined. Divide by $f''(x_n)$ and use

$$
x_{n+1}=x_n-\frac{f'(x_n)}{f''(x_n)}
$$

to obtain the exact error relation

$$
x^*-x_{n+1}
=-\frac{f'''(y_n)}{2f''(x_n)}(x^*-x_n)^2.
$$

The assumed derivative bounds now give the [quadratic convergence bound for Newton's method](../../../../../quadratic-convergence-bound-for-newton-s-method.md)

$$
\boxed{|x^*-x_{n+1}|
\leq\frac{C_2}{2C_1}|x^*-x_n|^2}
$$

for every $n$.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
