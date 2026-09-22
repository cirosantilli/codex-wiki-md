<h1 id="9c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Cartesian second-rank tensor](../../../../../../cartesian-second-rank-tensor.md) has components in every orthonormal Cartesian frame that transform according to

$$
A'_{ij}=Q_{ip}Q_{jq}A_{pq},\qquad A'=QAQ^T,
$$

when vector components transform as $x'=Qx$ for an [orthogonal matrix](../../../../../../orthogonal-matrix.md) $Q$. Repeated indices are summed. If $A=B$ in one frame, their transformed difference is $Q(A-B)Q^T=0$, so their equality holds in every such frame, at the same physical point.

Now impose the scalar contraction hypothesis on $C$. For every tensor $A$, invariance in the two frames says

$$
C'_{ij}Q_{ip}Q_{jq}A_{pq}=C_{pq}A_{pq}.
$$

At a fixed point, choose the components of $A$ to be each matrix unit in turn; each is an admissible tensor once its components in other frames are transformed. Thus every coefficient of $A_{pq}$ agrees, yielding $Q^TC'Q=C$, or

$$
\boxed{C'=QCQ^T.}
$$

Therefore **$C$ is necessarily a Cartesian second-rank tensor**. This is the [scalar contraction test for a Cartesian tensor](../../../../../../scalar-contraction-test-for-a-cartesian-tensor.md). Testing all tensors, rather than only symmetric tensors, is essential to the proof.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9C](../../9c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
