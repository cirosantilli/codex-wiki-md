<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Write $R=\mathbb Z[\sqrt{-13}]$ and $I=(2,1+\sqrt{-13})$. The map

$$
R\longrightarrow\mathbb F_2,
\qquad a+b\sqrt{-13}\longmapsto a+b\pmod2
$$

is a surjective [ring homomorphism](../../../../../ring-homomorphism.md): in $\mathbb F_2$, the image of $\sqrt{-13}$ is $1$ and $1^2=-13=1$. Its kernel is exactly $I$. Indeed, both generators lie in the kernel; conversely, if $a+b$ is even, then

$$
a+b\sqrt{-13}=b(1+\sqrt{-13})+(a-b),
$$

and $a-b$ is even. Hence $R/I\cong\mathbb F_2$ and the [index of a subgroup](../../../../../index-of-a-subgroup.md) is $[R:I]=2$.

If $I=(\alpha)$ were a [principal ideal](../../../../../principal-ideal.md), multiplication by $\alpha=a+b\sqrt{-13}$ would identify its additive lattice with a sublattice of index

$$
|N(\alpha)|=|\alpha\overline\alpha|=a^2+13b^2.
$$

Thus principality would require $a^2+13b^2=2$. This [Diophantine equation](../../../../../diophantine-equation.md) has no integer solution: $b=0$ would give $a^2=2$, while $b\ne0$ makes the left side at least $13$. Therefore

$$
\boxed{(2,1+\sqrt{-13})\text{ is not principal}}.
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
