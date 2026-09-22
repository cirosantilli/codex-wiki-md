<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [controlled-NOT gate](../../../../../../../controlled-not-gate.md) $U=\operatorname{CNOT}_{12}$, propagation of the Pauli generators gives

$$
\boxed{
UX_1U^\dagger=X_1X_2,
\qquad UX_2U^\dagger=X_2,
\qquad UZ_1U^\dagger=Z_1,
\qquad UZ_2U^\dagger=Z_1Z_2}.
$$

Thus an $X$ on the control propagates forward to the target, while a $Z$ on the target propagates backward to the control.

Suppose $\widetilde V$ has the same four conjugation rules and put $W=U^\dagger\widetilde V$. Then $W$ commutes with $X_1,X_2,Z_1,Z_2$. These generators span the full two-qubit operator algebra, so its [commutant](../../../../../../../centralizer.md) consists only of scalar multiples of the identity. Hence $W=e^{i\phi}I$ and

$$
\boxed{\widetilde V=e^{i\phi}U}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
