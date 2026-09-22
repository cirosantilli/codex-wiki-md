<h1 id="6e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the formal [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) to the molecule count: its increment is $+1$ at rate $\lambda$ and $-2$ at rate $\beta x^2$. Thus the exact first-moment identity for the specified generator is

$$
\boxed{\frac d{dt}\langle x\rangle=\lambda-2\beta\langle x^2\rangle
=\lambda-2\beta\big(\langle x\rangle^2+\operatorname{Var}x\big).}
$$

Neglecting fluctuations gives the [mean-field approximation](../../../../../../mean-field-approximation.md) $\dot m=\lambda-2\beta m^2$, so the positive steady mean is

$$
\boxed{m=\langle x\rangle\simeq\sqrt{\lambda/(2\beta)}.}
$$

There is a physical boundary qualification: the printed loss propensity is positive at $x=1$ and would produce a negative molecule count. Consequently it does not by itself define a molecule-count chain on all nonnegative integers. If losses are forbidden below two, the exact loss moment becomes $2\beta E[x^2\mathbf1_{\{x\geq2\}}]$; a mass-action two-molecule propensity instead uses $x(x-1)$. The calculation requested here uses the printed formal generator and its large-copy-number approximation, where such boundary corrections are negligible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6E](../../6e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
