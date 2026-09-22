<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use only the variable names $x,y$. Define mutually renamed formulas by

$$
D_1^x(x)=(x=x),\qquad
D_{m+1}^x(x)=\exists y\,[x<y\land D_m^y(y)],
$$

where $D_m^y$ is obtained from $D_m^x$ by globally interchanging $x$ and $y$, including their bound occurrences. By induction, $D_m^x(a)$ means that an increasing chain of $m$ elements starts at $a$. Hence

$$
\boxed{\lambda_n=\exists x\,D_n^x(x)\in L^2}
$$

holds exactly when the [linear order](../../../../../../linear-order.md) has at least $n$ elements. Inner quantifiers may bind the name $x$ again, but their scope is only the nested subformula; the comparison $x<y$ still refers to the preceding point. This [finite-variable logic](../../../../../../finite-variable-logic.md) construction works on finite and infinite [linear orders](../../../../../../linear-order.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
