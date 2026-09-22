<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the standard form $Cz\leq d$ with unrestricted $z=(x,y)^T$:

$$
C=\begin{pmatrix}-1&0\\1&-1\\1&1\end{pmatrix},
\qquad d=\begin{pmatrix}0\\1\\-2\end{pmatrix}.
$$

The nonnegative multiplier

$$
\boxed{w=\begin{pmatrix}2\\1\\1\end{pmatrix}}
$$

satisfies $C^Tw=0$ and $d^Tw=-1<0$. This is a [Farkas certificate for linear inequalities](../../../../../../farkas-certificate-for-linear-inequalities.md), so the system is infeasible by [Farkas' lemma](../../../../../../farkas-lemma.md). In scalar form, adding twice the first inequality to the other two produces

$$
\boxed{0\leq-1,}
$$

which directly exhibits the contradiction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
