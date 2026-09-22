<h1 id="14b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\Delta=\theta_1-\theta_2$ and $\omega_0^2=g/l$. The Euler--Lagrange equations, after division by the appropriate powers of $l$, are

$$
\boxed{(M+m)\ddot\theta_1+m\cos\Delta\,\ddot\theta_2
+m\sin\Delta\,\dot\theta_2^2+(M+m)\omega_0^2\sin\theta_1=0,}
$$



$$
\boxed{\ddot\theta_2+\cos\Delta\,\ddot\theta_1
-\sin\Delta\,\dot\theta_1^2+\omega_0^2\sin\theta_2=0.}
$$

Time-translation invariance conserves the total energy

$$
E=\frac12(M+m)l^2\dot\theta_1^2+\frac12ml^2\dot\theta_2^2
+ml^2\cos\Delta\,\dot\theta_1\dot\theta_2
-(M+m)gl\cos\theta_1-mgl\cos\theta_2.
$$

Setting both angles and velocities to zero satisfies the equations, so the downward configuration is an equilibrium. Writing $\theta_i=z_i$ and retaining linear terms gives

$$
\boxed{(M+m)\ddot z_1+m\ddot z_2+(M+m)\omega_0^2z_1=0,}
$$



$$
\boxed{\ddot z_1+\ddot z_2+\omega_0^2z_2=0.}
$$

Equivalently, the mass and stiffness matrices are

$$
\mathsf M=l^2\begin{pmatrix}M+m&m\\m&m\end{pmatrix},
\qquad
\mathsf K=gl\begin{pmatrix}M+m&0\\0&m\end{pmatrix}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
