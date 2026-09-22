<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep the printed coupling $g$ symbolic and use the [Dirac adjoint](../../../../../../dirac-adjoint.md) $\bar\psi=\psi^\dagger\gamma^0$ and $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$. Varying the action with respect to the independent adjoint variable gives the [Euler-Lagrange field equation](../../../../../../euler-lagrange-field-equation.md)

$$
\boxed{(i\gamma^\mu\partial_\mu-m-g\phi\gamma^5)\psi=0.}
$$

Varying with respect to $\psi$ and integrating its derivative term by parts gives the corresponding left-acting [adjoint Dirac equation](../../../../../../adjoint-dirac-equation.md)

$$
i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi+g\phi\bar\psi\gamma^5=0.
$$

Now differentiate the [axial current](../../../../../../axial-current.md) $j_5^\mu=\bar\psi\gamma^\mu\gamma^5\psi$. The first equation supplies $\gamma^\mu\partial_\mu\psi=-i(m+g\phi\gamma^5)\psi$, and the second supplies $(\partial_\mu\bar\psi)\gamma^\mu=i\bar\psi(m+g\phi\gamma^5)$. Since $\{\gamma^\mu,\gamma^5\}=0$ and $(\gamma^5)^2=1$,

$$
\begin{aligned}
\partial_\mu j_5^\mu
&=(\partial_\mu\bar\psi)\gamma^\mu\gamma^5\psi
+\bar\psi\gamma^\mu\gamma^5\partial_\mu\psi\\
&=i\bar\psi(m+g\phi\gamma^5)\gamma^5\psi
+i\bar\psi\gamma^5(m+g\phi\gamma^5)\psi.
\end{aligned}
$$

Therefore the [axial-current divergence for a pseudoscalar Yukawa interaction](../../../../../../axial-current-divergence-for-a-pseudoscalar-yukawa-interaction.md) is

$$
\boxed{\partial_\mu j_5^\mu=2im\bar\psi\gamma^5\psi+2ig\phi\bar\psi\psi.}
$$

Both the fermion mass and the interaction can break the axial symmetry. This is the classical field-equation identity being asked for, not a claim that quantum composite operators need no [renormalization](../../../../../../renormalization.md).

There is a convention issue in the original PDF: its interaction is written without an explicit $i$. The [Hermiticity of a pseudoscalar Dirac bilinear](../../../../../../hermiticity-of-a-pseudoscalar-dirac-bilinear.md) follows directly from

$$
(\bar\psi\gamma^5\psi)^\dagger=\psi^\dagger\gamma^5\gamma^0\psi
=-\psi^\dagger\gamma^0\gamma^5\psi=-\bar\psi\gamma^5\psi.
$$

For real $\phi$, the printed interaction is Hermitian if $g^*=-g$, rather than if $g$ is real. The PDF does not specify that $g$ is real, so a consistent physical convention is $g=i g_P$ with real $g_P$. Its interaction is $-i g_P\phi\bar\psi\gamma^5\psi$, and the divergence becomes $2im\bar\psi\gamma^5\psi-2g_P\phi\bar\psi\psi$. If $g$ were instead required to be real, the printed action would be non-Hermitian; the variational formulas above would still be formal calculations, but the variational adjoint equation would not be its Hermitian-conjugate equation. No missing factor is silently inserted into the solution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
