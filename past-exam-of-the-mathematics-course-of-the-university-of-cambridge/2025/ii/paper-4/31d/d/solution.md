<h1 id="31d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $v=e^S$ and $p=S'$. The [Liouville-Green exponential ansatz](../../../../../../liouville-green-exponential-ansatz.md) turns the normal-form equation into the [Riccati equation](../../../../../../riccati-equation.md)

$$
p'+p^2
=\frac14\left(1+\frac2x-\frac1{x^2}\right).
$$

Write

$$
p\sim b_0+\frac{b_1}{x}+\frac{b_2}{x^2}+\cdots.
$$

Matching the constant, $x^{-1}$, and $x^{-2}$ coefficients gives

$$
b_0^2=\frac14,\qquad
2b_0b_1=\frac12,\qquad
b_1^2+2b_0b_2-b_1=-\frac14.
$$

For the recessive branch,

$$
b_0=-\frac12,\qquad b_1=-\frac12,\qquad b_2=1,
$$

so

$$
S_-(x)
=-\frac x2-\frac12\log x-\frac1x+O(x^{-2}).
$$

Since $y=e^{x/2}x^{-1/2}v$, this gives

$$
y_-(x)
=x^{-1}\exp\left(-\frac1x+O(x^{-2})\right)
=\frac1x-\frac1{x^2}+O(x^{-3}).
$$

This agrees with the first two terms of part (a),

$$
U(x)\sim\frac1x-\frac1{x^2}+\frac2{x^3}-\cdots.
$$

Continuing the Riccati recursion reproduces the factorial asymptotic series, so $U$ is proportional to this recessive branch.

For the dominant branch,

$$
b_0=\frac12,\qquad b_1=\frac12,\qquad b_2=0,
$$

and in fact

$$
S_+(x)=\frac x2+\frac12\log x+\text{constant}
$$

solves the phase equation exactly. It follows that

$$
v_+(x)\asymp e^{x/2}x^{1/2},
\qquad
\boxed{y_+(x)\asymp e^x}.
$$

Indeed, $e^x$ is an exact second solution of the original differential equation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31D](../../31d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
