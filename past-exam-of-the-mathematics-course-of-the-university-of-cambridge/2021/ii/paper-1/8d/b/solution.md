<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Euler--Lagrange equations](../../../../../../euler-lagrange-equation.md) for the quadratic Lagrangian are

$$
m\ddot x+\mathsf Vx=0.
$$

For a [normal mode](../../../../../../normal-mode.md) $x(t)=a e^{i\omega t}$, they become the [generalized eigenvalue problem for small oscillations](../../../../../../generalized-eigenvalue-problem-for-small-oscillations.md)

$$
\mathsf Va=m\omega^2a.
$$

Put $\lambda=m\omega^2/k$. With the stated spring constants,

$$
\frac{\mathsf V}{k}
=
\begin{pmatrix}
1+\varepsilon(1+\delta)&-\varepsilon\\
-\varepsilon&1+\varepsilon(1-\delta)
\end{pmatrix}
=(1+\varepsilon)I
+\varepsilon
\begin{pmatrix}
\delta&-1\\
-1&-\delta
\end{pmatrix}.
$$

The final matrix has [characteristic polynomial](../../../../../../characteristic-polynomial.md)

$$
\nu^2-(1+\delta^2),
$$

so its [eigenvalue](../../../../../../eigenvalue.md) are $\nu_\pm=\pm\sqrt{1+\delta^2}$. Hence

$$
\lambda_\pm
=1+\varepsilon\pm\varepsilon\sqrt{1+\delta^2}
=1+\varepsilon\left(1\pm\sqrt{1+\delta^2}\right).
$$

The two [angular frequencies](../../../../../../angular-frequency.md) therefore satisfy

$$
\boxed{
\omega_\pm^2=\lambda_\pm\frac{k}{m},
\qquad
\lambda_\pm=1+\varepsilon\left(1\pm\sqrt{1+\delta^2}\right)
}.
$$

This is the spectrum recorded by [normal modes of two equal masses between three springs](../../../../../../normal-modes-of-two-equal-masses-between-three-springs.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
