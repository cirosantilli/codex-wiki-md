<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $\mathbf x_0$ is one solution. By [linearity](../../../../../../../linearity.md),

$$
A\mathbf x=\mathbf b
\iff A(\mathbf x-\mathbf x_0)=0
\iff\mathbf x-\mathbf x_0\in\ker T_A.
$$

Thus the [solution set of a linear system](../../../../../../../solution-set-of-a-linear-system.md) is exactly $\mathbf x_0+\ker T_A$. It has one member if the [kernel](../../../../../../../kernel-of-a-linear-map-split.md) is $\{0\}$. Conversely, if there is a unique solution and $\mathbf z\in\ker T_A$, then $\mathbf x_0+\mathbf z$ is also a solution, forcing $\mathbf z=0$. Combining this with [i](../i.md) gives

$$
\boxed{\text{unique solution}\iff\mathbf b\in\operatorname{im}T_A\text{ and }\ker T_A=\{0\}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
