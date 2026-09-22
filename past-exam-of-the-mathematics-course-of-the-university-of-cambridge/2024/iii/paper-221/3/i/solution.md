<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [nonparametric structural equation model](../../../../../../nonparametric-structural-equation-model.md) for the graph can be written

$$
X=f_X(U_X),\qquad A=f_A(U_A),\qquad
M=f_M(A,X,U_M),\qquad Y=f_Y(M,X,U_Y).
$$

The bidirected edge $A\leftrightarrow Y$ permits dependence between $U_A$ and $U_Y$; apart from this pair the exogenous variables are mutually independent. The basic [potential outcomes](../../../../../../potential-outcome.md) are

$$
M(a,x)=f_M(a,x,U_M),
\qquad
Y(m,x)=f_Y(m,x,U_Y),
$$

and the natural nested outcome is $Y(a)=Y(M(a,X),X)$.

The exogenous independences imply that the whole family $\{M(a,x):a,x\}$ is independent of $\{X,A,Y(m,x):m,x\}$, while $X$ is independent of $A$ and the basic response potentials. The bidirected edge means that $A$ and $Y(m,x)$ need not be independent. Useful observed-counterfactual consequences include

$$
M(a)\mathrel{\perp\!\!\!\perp}A\mid X,
\qquad
M\mathrel{\perp\!\!\!\perp}Y(m)\mid A,X.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
