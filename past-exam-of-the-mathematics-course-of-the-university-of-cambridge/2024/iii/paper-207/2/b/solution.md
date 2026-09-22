<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For equal arm size $n$, write $v^*=p_1(1-p_1)+p_0(1-p_0)$ at the clinically relevant alternative. A one-sided level-$\alpha$ [Wald test](../../../../../../wald-test.md) rejects when $Z>z_{1-\alpha}$, and its approximate [statistical power](../../../../../../statistical-power.md) is

$$
1-\Phi\!\left(z_{1-\alpha}-\frac{\delta^*\sqrt n}{\sqrt{v^*}}\right).
$$

Equating this to $1-\beta$ gives the per-arm [sample size](../../../../../../sample-size.md)

$$
n=\frac{v^*\bigl(z_{1-\alpha}+z_{1-\beta}\bigr)^2}{(\delta^*)^2},
$$

rounded up. If the design uses a null-based critical standard error $v_0$ but an alternative standard error $v^*$, the corresponding more general formula is

$$
\boxed{n=\frac{\bigl(z_{1-\alpha}\sqrt{v_0}+z_{1-\beta}\sqrt{v^*}\bigr)^2}{(\delta^*)^2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
