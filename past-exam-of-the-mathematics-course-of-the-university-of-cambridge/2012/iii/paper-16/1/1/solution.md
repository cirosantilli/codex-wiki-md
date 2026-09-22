<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The three [handle attachments](../../../../../../handle-attachment.md) give $H_2(W;\mathbb Z)\cong\mathbb Z^3$: there are no one-handles or three-handles. Use the capped [core disks of handles](../../../../../../core-disk-of-a-handle.md) as the [homology](../../../../../../homology-split.md) basis, ordered by the framing labels $-2,-1,+1$. The [surgery linking matrix](../../../../../../surgery-linking-matrix.md) gives the [intersection form](../../../../../../intersection-form.md). Orient the three components so that the outer components have [linking number](../../../../../../linking-number.md) $3$ and the middle component has [linking number](../../../../../../linking-number.md) $1$ with each outer component. There are six crossings between the outer components, and two crossings between the middle component and each outer component; counting their signs gives these [linking numbers](../../../../../../linking-number.md). Reversing a component changes the corresponding row and column signs and does not change the invariants.

Thus the **intersection form** is

$$
\boxed{Q_W=\begin{pmatrix}-2&1&3\\1&-1&1\\3&1&1\end{pmatrix}.}
$$

An exact [matrix congruence](../../../../../../matrix-congruence.md) diagonalizes this [intersection form](../../../../../../intersection-form.md) to

$$
\operatorname{diag}\left(-2,-\frac12,18\right).
$$

Consequently its **signature** is $\boxed{\sigma(W)=-1}$, and $\det Q_W=18$.

The [long exact sequence in relative homology](../../../../../../long-exact-sequence-in-relative-homology.md) and [Poincare-Lefschetz duality](../../../../../../lefschetz-duality.md) identify

$$
H_2(W)\longrightarrow H_2(W,\partial W)
$$

with the [intersection form](../../../../../../intersection-form.md) matrix, and identify $H_1(\partial W)$ with its [cokernel](../../../../../../cokernel.md), since $H_1(W)=0$. The [Smith normal form](../../../../../../smith-normal-form.md) has first invariant factor $1$, because the entries have greatest common divisor $1$, and second invariant factor $1$, because the upper-left two-by-two [matrix minor](../../../../../../minor-linear-algebra.md) has determinant $1$. The last invariant factor is $18$. Hence

$$
\boxed{H_1(\partial W;\mathbb Z)\cong\mathbb Z/18.}
$$

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
