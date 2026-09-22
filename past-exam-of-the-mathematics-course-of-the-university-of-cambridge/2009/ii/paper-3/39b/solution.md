<h1 id="39b/solution">Solution</h1>

↑ **Parent:** [39B](../39b.md)

Set $\theta_k=k\pi/(M+1)$ and extend the proposed vector by $v_0=v_{M+1}=0$. For $v_m=i^m\sin(m\theta_k)$, the angle-addition identity gives

$$
v_{m+1}-v_{m-1}=i^{m+1}[\sin((m+1)\theta_k)+\sin((m-1)\theta_k)]=2i\cos\theta_k\,v_m.
$$

Hence the [Toeplitz antisymmetric tridiagonal matrix](../../../../../toeplitz-antisymmetric-tridiagonal-matrix.md) has eigenvalues

$$
\boxed{\lambda_k=a+2ib\cos\frac{k\pi}{M+1},\qquad1\le k\le M.}
$$

The real sine vectors are eigenvectors of the real symmetric tridiagonal matrix with both off-diagonals one, with distinct eigenvalues $2\cos\theta_k$; thus they are orthogonal and form a basis. Multiplication by the unitary diagonal matrix $\operatorname{diag}(i,i^2,\ldots,i^M)$ preserves orthogonality. Their squared norms are $(M+1)/2$, so multiplying by $\sqrt{2/(M+1)}$ gives a common [orthonormal basis](../../../../../orthonormal-basis.md) for all $a,b$, even when some eigenvalues coincide.

Let $K$ have superdiagonal one, subdiagonal minus one and diagonal zero. The prescribed endpoint values remove the exterior unknowns, and the scheme is

$$
\boxed{B=I-\frac\mu4K,\qquad C=I+\frac\mu4K,\qquad Bu^{n+1}=Cu^n.}
$$

In the common orthonormal eigenbasis, the two eigenvalues are $1\mp i(\mu/2)\cos\theta_k$. Every eigenvalue of $B$ is nonzero for real $\mu$, and the amplification matrix $Q=B^{-1}C$ has eigenvalues

$$
q_k=\frac{1+i(\mu/2)\cos\theta_k}{1-i(\mu/2)\cos\theta_k},\qquad |q_k|=1.
$$

Thus $Q$ is a [unitary matrix](../../../../../unitary-matrix.md) and $\|u^{n+1}\|_2=\|u^n\|_2$ exactly. The same holds for the mesh-weighted norm. This matrix argument proves $\boxed{\text{stability for every real }\mu\text{, hence every physical }\mu\ge0}$, without a Fourier stability calculation.

**The printed mesh ratio has a consistency error:** advection requires $\mu=\Delta t/\Delta x$, while the PDF prints $\Delta t/(\Delta x)^2$. Indeed the centered spatial difference is $2\Delta x\,u_x+O((\Delta x)^3)$, so division of the scheme by $\Delta t$ gives leading right-hand coefficient $\mu\Delta x/\Delta t$. The printed choice makes this $1/\Delta x$ rather than one. The stability conclusion is valid for the algebraic scheme with either definition, but does not fix this inconsistency. The continuous first-order advection problem also ordinarily specifies only the inflow endpoint, here $x=1$; zero data at both endpoints restrict admissible initial data. For example the initially boundary-zero profile $\sin\pi x$ develops nonzero outflow $u(0,t)=\sin\pi t$ before inflow changes reach that boundary. The matrix norm calculation concerns the stated two-endpoint discretization and does not establish well-posedness for arbitrary continuous initial data.

## ↑ Ancestors (10)

1. [39B](../39b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
