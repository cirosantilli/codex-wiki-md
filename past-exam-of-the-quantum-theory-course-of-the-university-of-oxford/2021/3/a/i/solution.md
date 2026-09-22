<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [angular momentum eigenstates](../../../../../angular-momentum-eigenstate.md) have $J^2$ [eigenvalue](../../../../../eigenvalue.md) $\hbar^2j(j+1)$, where the [angular momentum quantum number](../../../../../angular-momentum-quantum-number.md) is $j=0,\tfrac12,1,\tfrac32,\ldots$. For each $j$, the [magnetic quantum number](../../../../../magnetic-quantum-number.md) runs in unit steps from $-j$ to $j$. Here that [magnetic quantum number](../../../../../magnetic-quantum-number.md) is $+1/2$, so only half-integer $j$ are compatible:

$$
\boxed{\lambda=j(j+1),\qquad j=\frac12,\frac32,\frac52,\ldots,\qquad
\lambda\in\left\{\frac34,\frac{15}4,\frac{35}4,\ldots\right\}.}
$$

Integer $j$ cannot contain a $J_3$ [eigenvalue](../../../../../eigenvalue.md) $\hbar/2$. Applying the [angular momentum lowering operator](../../../../../angular-momentum-lowering-operator.md) and using $[J_3,J_-]=-\hbar J_-$ gives

$$
J_3\varphi=J_3J_-\psi=(J_-J_3-\hbar J_-)\psi
=\boxed{-\frac\hbar2\varphi}.
$$

The lowered vector is nonzero, since the [adjoint operator](../../../../../adjoint-operator.md) identity $J_-^*=J_+$ gives

$$
\|\varphi\|^2=\langle\psi,J_+J_-\psi\rangle
=\hbar^2\left(\lambda-\frac14+\frac12\right)
=\hbar^2\left(\lambda+\frac14\right)>0.
$$

Finally, $J_3$ is a [self-adjoint operator](../../../../../self-adjoint-operator.md), so its [eigenstates](../../../../../eigenstate.md) for distinct [eigenvalues](../../../../../eigenvalue.md) are [orthogonal](../../../../../orthogonal-vectors.md). Explicitly,

$$
-\frac\hbar2\langle\varphi\mid\psi\rangle
=\langle J_3\varphi\mid\psi\rangle
=\langle\varphi\mid J_3\psi\rangle
=\frac\hbar2\langle\varphi\mid\psi\rangle,
$$

and hence $\boxed{\langle\varphi\mid\psi\rangle=0}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
