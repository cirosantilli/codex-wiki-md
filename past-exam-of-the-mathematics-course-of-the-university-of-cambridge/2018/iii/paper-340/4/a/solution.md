<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the usual definition, the [null space property](../../../../../../nullspace-property.md) relative to $S$ is $\|h_S\|_1<\|h_{S^c}\|_1$ for every nonzero $h\in\ker A$. It characterizes recovery by [basis pursuit](../../../../../../basis-pursuit.md) of every vector supported in $S$. Indeed, if it holds, then for any such $x_0$ and any nonzero $h\in\ker A$,

$$
\|x_0+h\|_1\ge\|x_0\|_1-\|h_S\|_1+\|h_{S^c}\|_1>\|x_0\|_1.
$$

Conversely, failure for some $h$ makes $x_0=-h_S$ and $z=h_{S^c}$ feasible with the same measurements and $\|z\|_1\le\|x_0\|_1$. Thus

$$
\boxed{\text{uniform recovery on }S\ \Longleftrightarrow\ \text{null space property on }S.}
$$

For the single fixed vector in the printing, necessity is false with that definition. For example,

$$
A=\begin{pmatrix}1&-1&0\\1&0&-1\end{pmatrix},\quad x_0=(1,-1,0),\quad S=\{1,2\}
$$

has $\ker A=\operatorname{span}\{(1,1,1)\}$. Along its feasible line, the objective is $|1+t|+|-1+t|+|t|$, uniquely minimized at $t=0$, although the [null space property](../../../../../../nullspace-property.md) would require $2<1$.

The correct [fixed-sign null space condition](../../../../../../fixed-sign-null-space-condition.md) is

$$
\boxed{|\langle\operatorname{sgn}(x_{0,S}),h_S\rangle|<\|h_{S^c}\|_1\quad(0\ne h\in\ker A).}
$$

Sufficiency follows from the supporting-line inequality for the [absolute value](../../../../../../absolute-value.md). Necessity follows by considering $x_0\pm th$ for small positive $t$, when all signs on $S$ remain unchanged: a nonpositive directional increase gives either a decrease or another minimizer. If “relative to $S$” was intended to include these signs, this is the precise condition needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
