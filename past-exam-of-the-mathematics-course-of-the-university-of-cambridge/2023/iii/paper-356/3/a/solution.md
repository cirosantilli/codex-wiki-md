<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [stochastic mass-action propensities](../../../../../../stochastic-chemical-kinetics.md)

$$
a_1=\frac{\alpha_1}{V}y(y-1),
\quad a_2=\frac{\alpha_2}{V}x(x-1),
\quad a_3=\frac{\alpha_3V}{\varepsilon},
\quad a_4=\frac{\alpha_4}{\varepsilon V}xy.
$$

Writing $E_x^rf(x,y)=f(x+r,y)$ and similarly for $E_y$, the fast and slow forward operators are

$$
\boxed{\mathcal L_0^*
=(E_y^{-1}-1)\alpha_3V
+(E_y^{+1}-1)\frac{\alpha_4xy}{V},}
$$



$$
\boxed{\mathcal L_1^*
=(E_x^{-1}E_y^{+2}-1)\frac{\alpha_1y(y-1)}V
+(E_x^{+1}-1)\frac{\alpha_2x(x-1)}V.}
$$

Each shift operator acts on everything to its right, including the propensity. Birth of $Y$ and consumption of $Y$ by $X+Y\to X$ are fast; $2Y\to X$ and $2X\to X$ are slow. The slow species is $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
