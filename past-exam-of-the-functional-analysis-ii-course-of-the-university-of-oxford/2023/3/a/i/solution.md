<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $A=\lambda I-T$. Since $T$ is a [self-adjoint operator](../../../../../self-adjoint-operator.md), $A^*=\overline\lambda I-T$. Applying the preceding [image-kernel orthogonality for an adjoint](../../../../../image-kernel-orthogonality-for-an-adjoint.md) identities to $A^*$ gives

$$
\overline{\operatorname{Im}A}=(\ker A^*)^\perp.
$$

If $\lambda$ is real, $A^*=A$ and $\ker A=\{0\}$ because $\lambda$ is not an [eigenvalue](../../../../../eigenvalue.md). If $\lambda$ is nonreal and $A^*x=0$, then $Tx=\overline\lambda x$. The scalar $\langle Tx,x\rangle$ is real by [self-adjointness](../../../../../self-adjoint-operator.md), while it equals $\overline\lambda\|x\|^2$. Its imaginary part forces $x=0$. Thus $\ker A^*=\{0\}$ in both cases, and

$$
\boxed{\overline{\operatorname{Im}(\lambda I-T)}=X.}
$$

The conjugation on $\lambda$ in the [adjoint operator](../../../../../adjoint-operator.md) is essential when $\lambda$ is nonreal.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
