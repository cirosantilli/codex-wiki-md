<h1 id="21i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $A=T-\lambda I$. We first prove that $\operatorname{im}A$ is dense. Otherwise some nonzero $y$ lies in its [orthogonal complement](../../../../../../orthogonal-complement.md), so

$$
A^*y=0,
\qquad T^*y=\overline\lambda y.
$$

By part (b), choose finite-dimensional spaces $E_j$ containing $y$ such that $S_j=P_{E_j}T\to T$ in [operator norm](../../../../../../operator-norm.md). Since

$$
S_j^*y=T^*P_{E_j}y=T^*y=\overline\lambda y,
$$

the operator $S_j^*-\overline\lambda I$ is not injective. Therefore $S_j-\lambda I$ is not surjective; the contrapositive of part (c) makes $\lambda$ an eigenvalue of $S_j$. Choose unit vectors $x_j$ with $S_jx_j=\lambda x_j$. Then

$$
\|Tx_j-\lambda x_j\|
\leq\|T-S_j\|\longrightarrow0.
$$

Compactness gives a subsequence for which $Tx_j$ converges. Since $\lambda\ne0$, the displayed relation makes $x_j$ converge to a unit vector $x$, and continuity gives $Tx=\lambda x$, contradicting the hypothesis. Thus $\operatorname{im}A$ is dense.

Next suppose $A$ were not bounded below, or equivalently that its [lower norm](../../../../../../lower-norm-of-an-operator.md) were zero. There would be unit vectors $x_j$ with $Ax_j\to0$, hence

$$
Tx_j=\lambda x_j+o(1).
$$

Again a convergent subsequence of $Tx_j$ forces the corresponding $x_j$ to converge to a unit vector $x$ satisfying $Ax=0$, another contradiction. Therefore some $c>0$ satisfies

$$
\|(T-\lambda I)x\|\geq c\|x\|.
$$

This lower bound makes $\operatorname{im}A$ closed: if $Ax_j$ converges, then $x_j$ is Cauchy and its limit maps to the same limit. Since the image is both dense and closed, it is all of $H$. We have proved the [Fredholm alternative for a compact operator](../../../../../../fredholm-alternative.md): every nonzero spectral value of a compact operator is an eigenvalue.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [21I](../../21i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
