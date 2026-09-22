<h1 id="b/5/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Stationarity of the equality-constrained quadratic model gives $g_k+H_ks_k-A_k^Ty_{k+1}=0$, while feasibility gives $A_ks_k=-c_k$. A symmetric system linking the step and new multiplier is

$$
\boxed{\begin{pmatrix}H_k&-A_k^T\\-A_k&0\end{pmatrix}\begin{pmatrix}s_k\\y_{k+1}\end{pmatrix}=\begin{pmatrix}-g_k\\c_k\end{pmatrix}.}
$$

Let $Z$ have columns forming a [basis](../../../../../basis.md) of $\ker A_k$. The [saddle-point matrix](../../../../../saddle-point-matrix.md) is nonsingular exactly when **$A_k$ has full row rank and $Z^TH_kZ$ is nonsingular**. Full row rank is necessary because a nonzero vector in $\ker A_k^T$ would give a null vector of the block matrix. Under full row rank, solving a homogeneous system forces $s=Zq$ and then $Z^TH_kZq=0$; this proves sufficiency and the converse. Positive definiteness of the [reduced Hessian](../../../../../reduced-hessian.md) is sufficient for a constrained minimum but is stronger than the nonsingularity condition asked here.

A null-space method first finds $s_p$ with $A_ks_p=-c_k$, then solves

$$
Z^TH_kZq=-Z^T(g_k+H_ks_p),\qquad s_k=s_p+Zq,
$$

and recovers $y_{k+1}$ from $A_k^Ty_{k+1}=g_k+H_ks_k$. It needs the stated full row rank and nonsingular reduced matrix; [Cholesky decomposition](../../../../../cholesky-decomposition.md) is available when the latter is positive definite.

A range-space method additionally assumes $H_k$ is invertible. It solves the [Schur complement](../../../../../schur-complement.md) equations

$$
A_kH_k^{-1}A_k^Ty_{k+1}=A_kH_k^{-1}g_k-c_k,
\qquad s_k=-H_k^{-1}g_k+H_k^{-1}A_k^Ty_{k+1}.
$$

If $H_k$ is positive definite and $A_k$ has full row rank, the Schur matrix is positive definite and both solves can use [Cholesky decomposition](../../../../../cholesky-decomposition.md). An indefinite but invertible $H_k$ instead requires a suitable indefinite factorization; the Schur matrix must remain nonsingular.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
