<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\sigma=\operatorname{sgn}(x_S)$, using the real [sign function](../../../../../../sign-function.md) on the [support of a vector](../../../../../../support-of-a-vector.md) $x$. The [fixed-sign null space condition](../../../../../../fixed-sign-null-space-condition.md) in the PDF uses $S^c$ on its right-hand side. This complement is essential. For any real coordinate $x_j\ne0$, the supporting-line inequality for the [absolute value](../../../../../../absolute-value.md) is

$$
|x_j+v_j|\ge|x_j|+\operatorname{sgn}(x_j)v_j.
$$

Every distinct feasible [vector](../../../../../../vector.md) is $x+v$ with $0\ne v\in\ker A$. Summing the coordinate inequalities on $S$ and adding the [L1 norm](../../../../../../l1-norm.md) on $S^c$ gives

$$
\|x+v\|_1-\|x\|_1\ge\langle\sigma,v_S\rangle+\|v_{S^c}\|_1\ge\|v_{S^c}\|_1-|\langle\sigma,v_S\rangle|>0.
$$

The strict final inequality is precisely the [fixed-sign null space condition](../../../../../../fixed-sign-null-space-condition.md). **Hence $x$ is the unique [basis pursuit](../../../../../../basis-pursuit.md) [minimizer](../../../../../../global-minimizer.md).** Unlike the [null space property](../../../../../../nullspace-property.md) of Question 1, this condition concerns the particular [sign function](../../../../../../sign-function.md) values of $x$, rather than every [vector](../../../../../../vector.md) supported in $S$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
