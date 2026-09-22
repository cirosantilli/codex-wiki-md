<h1 id="34b/solution">Solution</h1>

↑ **Parent:** [34B](../34b.md)

If $Lf=\lambda f$ and $f_t+Af=0$, [differentiation](../../../../../differentiation.md) and the [Lax equation](../../../../../isospectral-lax-equation.md) give $(L-\lambda)f_t=-A(L-\lambda)f$, so $\lambda_t=0$ after projection onto the normalized [eigenfunction](../../../../../eigenfunction.md) for a [nondegenerate eigenvalue](../../../../../simple-eigenvalue.md).

For $\Psi=(f,f_x)^T$,

$$
M_L=\begin{pmatrix}0&1\\u-\lambda&0\end{pmatrix},
$$



$$
M_A=\begin{pmatrix}-u_x-b&-(u-\lambda+a)\\-u_{xx}-b_x-(u-\lambda+a)(u-\lambda)&-2u_x-b-a_x\end{pmatrix}.
$$

The compatibility $\Psi_{xt}=\Psi_{tx}$ is precisely $\partial_tM_L-\partial_xM_A-[M_A,M_L]=0$. If all coefficients are $x$-independent, this becomes $\dot M_L=[M_A,M_L]$, and cyclicity of trace gives $d\operatorname{Tr}(M_L^k)/dt=0$.

## ↑ Ancestors (10)

1. [34B](../34b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
