<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [characteristic polynomial](../../../../characteristic-polynomial.md) of $M$ is

$$
\det(\lambda I-M)=(\lambda-6)(\lambda-3)+2=(\lambda-4)(\lambda-5).
$$

The corresponding [eigenvectors](../../../../eigenvector.md) may be chosen as $v_4=(1,2)^T$ and $v_5=(1,1)^T$. They are linearly independent, so write $\boldsymbol x=q_4(t)v_4+q_5(t)v_5$. Substitution in the system of [ordinary differential equations](../../../../ordinary-differential-equation.md) gives

$$
(q_4''+4q_4)v_4+(q_5''+5q_5)v_5=0.
$$

Independence of the [eigenvectors](../../../../eigenvector.md) yields two decoupled [harmonic oscillator equations](../../../../simple-harmonic-motion.md). Their four integration constants give the general real solution

$$
\boxed{\boldsymbol x(t)=
\begin{pmatrix}1\\2\end{pmatrix}(A\cos2t+B\sin2t)
+\begin{pmatrix}1\\1\end{pmatrix}(C\cos(\sqrt5t)+D\sin(\sqrt5t)).}
$$

Both components can be differentiated directly to verify $\boldsymbol x''+M\boldsymbol x=0$. Orthogonality of the [eigenvectors](../../../../eigenvector.md) is unnecessary: diagonalizing this nonsymmetric [matrix](../../../../matrix.md) requires an invertible [eigenbasis](../../../../eigenbasis.md), not an orthonormal one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [12](../../12.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
