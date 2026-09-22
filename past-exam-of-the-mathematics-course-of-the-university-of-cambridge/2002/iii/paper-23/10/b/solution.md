<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a variable name $y\ne x$ among the $k$ available names and define

$$
C_1^x(x)=\phi(x),\qquad
C_{m+1}^x(x)=\phi(x)\land\exists y\,[x<y\land C_m^y(y)].
$$

The formula $C_m^y$ is obtained by interchanging the names $x,y$ throughout $C_m^x$, including bound occurrences. Its only free variable is $y$. A permutation of variable names preserves membership in $L^k$, so every formula in this recursion still uses at most the original $k$ names. In particular, bound variables inside a copy of $\phi$ do not accidentally capture the previous comparison: their scope stays inside that copy.

Induction proves that $C_m^x(a)$ holds exactly when there is an increasing $m$-tuple of satisfying elements whose first entry is $a$. Any set of $m$ distinct points in a [linear order](../../../../../../linear-order.md) can be put in increasing order. Therefore the [variable-recycling count on a linear order](../../../../../../variable-recycling-count-on-a-linear-order.md)

$$
\boxed{\phi_n=\exists x\,C_n^x(x)\in L^k}
$$

is the required sentence. This does not use counting quantifiers or additional variable names, and it applies equally to infinite [linear orders](../../../../../../linear-order.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
