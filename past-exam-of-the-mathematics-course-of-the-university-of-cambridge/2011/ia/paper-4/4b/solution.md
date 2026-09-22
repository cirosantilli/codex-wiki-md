<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

Write the standard [Lorentz transformation](../../../../../lorentz-transformation.md) as $x'=\gamma(x-vt)$, $ct'=\gamma(ct-vx/c)$, with [Lorentz factor](../../../../../lorentz-factor.md) $\gamma=(1-v^2/c^2)^{-1/2}$ and $|v|<c$. In the [null coordinates in two-dimensional Minkowski spacetime](../../../../../null-coordinates-in-two-dimensional-minkowski-spacetime.md), addition and subtraction give

$$
x'_+=\gamma(1-v/c)x_+,\qquad x'_-=\gamma(1+v/c)x_-.
$$

Since both factors are positive,

$$
\boxed{x'_+=\lambda(v)x_+,\quad x'_-=\lambda(-v)x_-,\qquad
\lambda(v)=\sqrt{\frac{c-v}{c+v}}.}
$$

Their product is one, so [Lorentz invariance](../../../../../lorentz-invariance.md) of the interval follows immediately:

$$
\boxed{x'^2-c^2t'^2=x'_+x'_-=x_+x_-=x^2-c^2t^2.}
$$

Two successive collinear [Lorentz boosts](../../../../../lorentz-boost.md) multiply the positive-coordinate factor by $\lambda(v_2)\lambda(v_1)$ and the negative-coordinate factor by its reciprocal. Thus they have the same form with a velocity $v_3$ determined by

$$
\frac{c-v_3}{c+v_3}
=\frac{(c-v_1)(c-v_2)}{(c+v_1)(c+v_2)}.
$$

Cross multiplication yields the [relativistic velocity-addition formula](../../../../../velocity-addition-formula.md) formula

$$
\boxed{v_3=\frac{v_1+v_2}{1+v_1v_2/c^2}.}
$$

For $|v_1|,|v_2|<c$, the denominator is positive and

$$
1-\frac{v_3^2}{c^2}
=\frac{(1-v_1^2/c^2)(1-v_2^2/c^2)}{(1+v_1v_2/c^2)^2}>0,
$$

so $v_3$ is admissible. The positive square roots then verify the factor identity itself, not merely its square. In terms of [rapidity](../../../../../rapidity.md) $v/c=\tanh\eta$, this same calculation is addition of rapidities because $\lambda(v)=e^{-\eta}$.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
