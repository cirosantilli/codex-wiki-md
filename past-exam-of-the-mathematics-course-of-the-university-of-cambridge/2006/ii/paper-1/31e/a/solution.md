<h1 id="31e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $E=e^{-ikx+k^2t}$. Expanding $\partial_t(Eq)+\partial_x(EX)$ shows that the required flux is

$$
\boxed{X=-q_x-ikq.}
$$

Indeed $X_x-ikX=-q_{xx}-k^2q$, cancelling the $k^2q$ from the time [derivative](../../../../../../derivative.md). Introduce a potential $\varphi$ by $\varphi_x=Eq$, $\varphi_t=E(q_x+ikq)$. Equality of its mixed [derivatives](../../../../../../derivative.md) is precisely the conservation law. With $\varphi=E\mu$, these equations become the linear auxiliary system

$$
\boxed{\mu_x-ik\mu=q,\qquad\mu_t+k^2\mu=q_x+ikq.}
$$

This is a [Lax pair](../../../../../../lax-pair.md) in the affine-potential form used for linear evolution equations. If a homogeneous [matrix](../../../../../../matrix.md) pair is preferred, set $\Psi=(\mu,1)^T$ and use $\Psi_x=\left(\begin{smallmatrix}ik&q\\0&0\end{smallmatrix}\right)\Psi$, $\Psi_t=\left(\begin{smallmatrix}-k^2&q_x+ikq\\0&0\end{smallmatrix}\right)\Psi$. Its [zero-curvature condition](../../../../../../zero-curvature-condition.md) has upper-right entry $q_t-q_{xx}$ and all other entries zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31E](../../31e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
