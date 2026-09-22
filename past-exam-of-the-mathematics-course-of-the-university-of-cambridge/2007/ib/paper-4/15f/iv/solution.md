<h1 id="15f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $F=\mathcal Lf$. Using the [Laplace transform of a derivative](../../../../../../laplace-transform-of-a-derivative.md) and the initial data gives

$$
\mathcal L(f^{(4)})=s^4F-1,\qquad\mathcal L(f^{(3)})=s^3F,\qquad\mathcal L(f'')=s^2F.
$$

The transformed equation is $(s^4+2s^3+s^2)F=1$, so $F=1/[s^2(s+1)^2]$. The preceding inverse [Laplace transform](../../../../../../laplace-transform.md) therefore gives

$$
\boxed{f(t)=t-2+(t+2)e^{-t}.}
$$

For a direct check, $f'=1-(t+1)e^{-t}$, $f''=te^{-t}$, $f^{(3)}=(1-t)e^{-t}$, and $f^{(4)}=(t-2)e^{-t}$. These satisfy both the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) and all four [initial conditions](../../../../../../initial-condition.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [15F](../../15f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
