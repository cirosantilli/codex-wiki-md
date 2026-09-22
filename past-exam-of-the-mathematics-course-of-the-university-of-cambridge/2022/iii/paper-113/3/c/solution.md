<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $A=k[x_1,x_2,x_3]$ and cover the [punctured affine three-space](../../../../../../punctured-affine-three-space.md) $X$ by the three [principal opens](../../../../../../principal-open-subscheme.md) $D(x_i)$. Every finite intersection is affine, so the [acyclic cover theorem](../../../../../../leray-s-theorem.md) identifies [sheaf cohomology](../../../../../../sheaf-cohomology.md) with the cohomology of

$$
0\longrightarrow\bigoplus_iA_{x_i}\longrightarrow\bigoplus_{i<j}A_{x_ix_j}\longrightarrow A_{x_1x_2x_3}\longrightarrow0.
$$

The augmented complex has zeroth cohomology $A$ and first cohomology zero. Its second cohomology is

$$
\frac{A_{x_1x_2x_3}}{A_{x_1x_2}+A_{x_1x_3}+A_{x_2x_3}},
$$

with $k$-basis represented by $x_1^{-a}x_2^{-b}x_3^{-c}$ for $a,b,c\geq1$. There are no higher Čech terms. Hence

$$
\boxed{H^q(X,\mathcal O_X)=
\begin{cases}
A,&q=0,\\
0,&q=1\text{ or }q\geq3,\\
\displaystyle\bigoplus_{a,b,c\geq1}k\,x_1^{-a}x_2^{-b}x_3^{-c},&q=2.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
