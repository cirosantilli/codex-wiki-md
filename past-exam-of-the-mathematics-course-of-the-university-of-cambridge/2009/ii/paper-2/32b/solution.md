<h1 id="32b/solution">Solution</h1>

↑ **Parent:** [32B](../32b.md)

Use a common invariant operator domain on which the stated differentiations and [commutator](../../../../../commutator.md) are valid. For a differentiable normalized [eigenfunction](../../../../../eigenfunction.md), the Hellmann-Feynman calculation and self-adjointness give

$$
\lambda'=\langle f,L_tf\rangle=\langle f,LAf-ALf\rangle
=\lambda\langle f,Af\rangle-\lambda\langle f,Af\rangle=0.
$$

The [Lax equation preserves the spectrum](../../../../../lax-equation-preserves-the-spectrum.md). Differentiating $Lf=\lambda f$ now gives $(L-\lambda)(f_t+Af)=0$, so $f_t+Af$ is in the same eigenspace, or is zero. For a nondegenerate [eigenvalue](../../../../../eigenvalue.md) it equals $c(t,\lambda)f$. Multiplying $f$ by $\exp[-\int c(t,\lambda)\,dt]$ produces $\widehat f$ with $\widehat f_t+A\widehat f=0$ while preserving its [eigenvalue](../../../../../eigenvalue.md).

Write $b=u_x+a_0$ and $d=u-\lambda+a_1$. The spatial [eigenvalue](../../../../../eigenvalue.md) equation gives $\widehat f_{xx}=(u-\lambda)\widehat f$, so $A\widehat f=b\widehat f+d\widehat f_x$. For $F=(\widehat f,\widehat f_x)^T$ the two first-order systems are therefore

$$
\boxed{U=\begin{pmatrix}0&1\\u-\lambda&0\end{pmatrix},\qquad
V=\begin{pmatrix}-b&-d\\-b_x-d(u-\lambda)&-b-d_x\end{pmatrix}.}
$$

The second row of $V$ follows by differentiating the first time equation in $x$ and using the spatial equation once more. Conversely these [matrix](../../../../../matrix.md) equations imply both scalar equations, so the formulations are equivalent.

## ↑ Ancestors (10)

1. [32B](../32b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
