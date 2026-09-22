<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Krylov subspace](../../../../krylov-subspace.md) is $\boxed{K_k(A,r)=\operatorname{span}\{r,Ar,\ldots,A^{k-1}r\}}$. If $y-z=q(A)r$ for a polynomial $q$ of degree at most $k-1$, then

$$
b-Ay=r-Aq(A)r=p(A)r,\qquad p(t)=1-tq(t),
$$

so $\deg p\leq k$ and $p(0)=1$. Conversely, this residual identity implies

$$
A\bigl(y-z-q(A)r\bigr)=0,\qquad q(t)=\frac{1-p(t)}t\in\Pi_{k-1}.
$$

Thus the converse holds whenever $A$ is invertible. More precisely, for fixed $A,r,k$ it holds for every such $y$ exactly when $\ker A\subseteq K_k(A,r)$: the identity determines $y-z$ only up to an arbitrary [nullspace](../../../../kernel-of-a-linear-map-split.md) vector. Without this qualification the singular-matrix converse is false, for example when $A=0$, $r=e_1$ and $y-z=e_2$.

Assume $r\ne0$ and exact arithmetic for the [Lanczos algorithm](../../../../lanczos-algorithm.md). At step $j$ put

$$
w=Av_j-\delta_jv_j-\gamma_jv_{j-1},\quad\delta_j=v_j^TAv_j,\quad\gamma_{j+1}=\|w\|_2,\quad v_{j+1}=w/\gamma_{j+1},
$$

provided $w\ne0$. The initial coefficient of $v_0=0$ is immaterial. Inductively suppose $v_1,\ldots,v_j$ are orthonormal. Then $v_j^Tw=0$ by the choice of $\delta_j$. For $j>1$, symmetry and the preceding recurrence give $v_{j-1}^TAv_j=\gamma_j$, so $v_{j-1}^Tw=0$. If $i\leq j-2$, the recurrence gives $Av_i\in\operatorname{span}(v_1,\ldots,v_{i+1})$, and therefore $v_i^TAv_j=(Av_i)^Tv_j=0$. Hence $w$ is perpendicular to every preceding basis vector. Its normalization supplies the next orthonormal vector.

Every new $v_{j+1}$ belongs to $K_{j+1}(A,r)$. The $j+1$ orthonormal vectors are independent, whereas that [Krylov subspace](../../../../krylov-subspace.md) has dimension at most $j+1$; they therefore form its basis. Continuing the recurrence one more step gives

$$
\boxed{AV_k=V_kT_k+\gamma_{k+1}v_{k+1}e_k^T,\quad
T_k=\begin{pmatrix}
\delta_1&\gamma_2&&\\
\gamma_2&\delta_2&\ddots&\\
&\ddots&\ddots&\gamma_k\\
&&\gamma_k&\delta_k
\end{pmatrix}.}
$$

In particular $T_k=V_k^TAV_k$. If the next residual is zero, the last term is zero and the span is an invariant subspace; no undefined normalized vector is needed. If $v_1$ is an [eigenvector](../../../../eigenvector.md), $Av_1=\delta_1v_1$, so $\gamma_2=0$ immediately. The algorithm terminates with the exact one-dimensional invariant subspace, rather than generating further vectors. If $r=0$, the initial residual has already vanished and the normalization defining $v_1$ is unnecessary.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
