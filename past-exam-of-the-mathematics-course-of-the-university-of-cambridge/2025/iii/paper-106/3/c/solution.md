<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor $T=AB$ as in part b(v). Then [Parseval identity for a Hilbertian basis](../../../../../../parseval-identity-for-a-hilbertian-basis.md) and [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\sum_n|\langle Te_n,e_n\rangle|
=\sum_n|\langle Be_n,A^*e_n\rangle|
\leq\|B\|_2\|A^*\|_2
=\|T\|_1.
$$

The defining series for the [operator trace](../../../../../../operator-trace.md) is therefore absolutely convergent and satisfies $|\operatorname{tr}T|\leq\|T\|_1$.

For unit vectors $x,y$, the [adjoint operator](../../../../../../adjoint-operator.md) of $R=x\otimes y$ is $R^*=y\otimes x$, and

$$
R^*R=y\otimes y=P_{\mathbb Cy}.
$$

Hence $|R|=P_{\mathbb Cy}$ and part b(iii), followed by Parseval, gives

$$
\|R\|_1
=\sum_n\langle P_{\mathbb Cy}e_n,e_n\rangle
=\sum_n|\langle e_n,y\rangle|^2=1.
$$

Scaling proves $\|x\otimes y\|_1=\|x\|\|y\|$. A second use of Parseval yields

$$
\operatorname{tr}(x\otimes y)
=\sum_n\langle e_n,y\rangle\langle x,e_n\rangle
=\langle x,y\rangle,
$$

which proves the asserted [rank-one operator](../../../../../../rank-one-operator.md) formulas.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
