<h1 id="7a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The forcing vector has the [eigenvector](../../../../../../eigenvector.md) decomposition

$$
(-\lambda,1,\lambda)^T
=\frac{\lambda+1}{2}v_-+\frac{\lambda-1}{2}v_+.
$$

There is no component in the zero [eigenvalue](../../../../../../eigenvalue.md) direction. The scalar [inhomogeneous linear differential equations](../../../../../../inhomogeneous-linear-differential-equation.md) in this basis are

$$
\dot z_-=-2z_-+(\lambda+1)e^{2t},\qquad
\dot z_0=0,\qquad
\dot z_+=2z_++(\lambda-1)e^{2t}.
$$

For the first, a [particular solution](../../../../../../particular-solution.md) is $(\lambda+1)e^{2t}/4$. For the third, multiplying by the [integrating factor](../../../../../../integrating-factor.md) $e^{-2t}$ gives $(e^{-2t}z_+)'=\lambda-1$. Consequently **for every real $\lambda$**

$$
\boxed{\begin{pmatrix}x\\y\\z\end{pmatrix}
=\left(Ae^{-2t}+\frac{\lambda+1}{4}e^{2t}\right)v_-
+Bv_0+\bigl(C+(\lambda-1)t\bigr)e^{2t}v_+.}
$$

When $\lambda=1$, the resonant component vanishes and a [particular solution](../../../../../../particular-solution.md) is $\tfrac12v_-e^{2t}$, of the stipulated constant-vector form. If $\lambda\ne1$, substituting $ce^{2t}$ would require $(2I-M)c=2(-\lambda,1,\lambda)^T$. In the [eigenbasis](../../../../../../eigenbasis.md) the left side has zero $v_+$ component, while the right side has component $\lambda-1$. This is impossible. The factor $t$ is therefore unavoidable: it is [resonance in a differential equation](../../../../../../resonance-in-a-differential-equation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7A](../../7a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
