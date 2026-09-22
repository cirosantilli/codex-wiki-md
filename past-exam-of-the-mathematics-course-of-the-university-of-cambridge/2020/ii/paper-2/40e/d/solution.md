<h1 id="40e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $A$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), it has a positive-definite inverse square root. Choose the [exact inverse-square-root preconditioner](../../../../../../exact-inverse-square-root-preconditioner.md)

$$
\boxed{P=A^{-1/2}}.
$$

Then

$$
PAP^T=A^{-1/2}AA^{-1/2}=I,
$$

which has one distinct eigenvalue, so preconditioned CG terminates in one step.

This construction is of little computational use because obtaining and applying $A^{-1/2}$ is generally at least as expensive in storage and arithmetic as directly factoring or solving the original system. A useful preconditioner must only approximate this transformation while remaining cheap to construct and apply.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
