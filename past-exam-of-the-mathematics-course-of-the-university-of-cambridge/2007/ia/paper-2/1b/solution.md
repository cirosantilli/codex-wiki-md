<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

The differential operator is $(D-3)^2$, where $D=d/dx$. Factoring out the forcing's exponential removes this repeated [characteristic root of a constant-coefficient differential equation](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md): set $y=e^{3x}v$. Differentiation gives $(D-3)y=e^{3x}v'$ and $(D-3)^2y=e^{3x}v''$, so $v''=\cos(2x)$. Two integrations yield

$$
v=-\frac14\cos(2x)+Ax+B.
$$

The [initial conditions](../../../../../initial-condition.md) become $v(0)=0$ and $v'(0)+3v(0)=1$, hence $B=1/4$ and $A=1$. Thus

$$
\boxed{y(x)=e^{3x}\left[x+\frac{1-\cos(2x)}4\right].}
$$

The factorization verifies the [differential equation](../../../../../differential-equation-split.md) directly, and the displayed expression has the required value and derivative at zero.

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
