<h1 id="19d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A full [QR decomposition](../../../../../../qr-decomposition.md) of a real $m$ by $n$ [matrix](../../../../../../matrix.md) with $m\ge n$ writes

$$
A=Q\begin{pmatrix}R\\0\end{pmatrix},
$$

where $Q$ is an orthogonal $m$ by $m$ [matrix](../../../../../../matrix.md) and $R$ is upper triangular $n$ by $n$. In the full-column-rank case $R$ is invertible. Equivalently the reduced factorization is $A=Q_1R$ with $Q_1^TQ_1=I_n$. Householder transformations can construct the full factorization.

Let $Q^Tb=\binom{c_1}{c_2}$ with $c_1\in\mathbb R^n$. Since orthogonal transformations preserve the [Euclidean norm](../../../../../../euclidean-norm.md),

$$
\|Ax-b\|_2^2=\|Rx-c_1\|_2^2+\|c_2\|_2^2.
$$

Therefore the [linear least-squares problem](../../../../../../linear-least-squares-problem.md) has the full-rank solution

$$
\boxed{Rx^*=c_1,\qquad \min_x\|Ax-b\|_2=\|c_2\|_2.}
$$

Back substitution solves this triangular system without forming $A^TA$. If the [matrix](../../../../../../matrix.md) is rank deficient, use a rank-revealing pivoted factorization and minimize over its independent columns; the minimizer need not be unique. The original PDF minimizes over $x\in\mathbb R^n$; the converted TeX's minimization over $b$ is a transcription error.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19D](../../19d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
