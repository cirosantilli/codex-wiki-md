<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $P$ now denote the degree-zero torsion [line bundle](../../../../../../line-bundle.md) represented by the point of $A[N]$, and put $L_P=\mathcal O_C(2K_C)\otimes P$. Again the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) gives $h^0(L_P)=n$ and $h^1(L_P)=0$. For translation, use $\Theta_P=\Theta+P$ as a translated subset. With ordinary $T_P(x)=x+P$, this is $T_{-P}^*\Theta$; the notation $t_P^*\Theta=\Theta+P$ therefore uses $t_P=T_{-P}$.

Let $s_P$ and $s_0$ be the evaluation [determinants](../../../../../../determinant.md) for the two chosen bases, interpreted as sections of $\det E_{L_P}$ and $\det E_L$. The kernel for the first determinant is $H^0(C,2K_C+P-\sum z_j)$. By [Serre duality](../../../../../../serre-duality.md) and the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) its dimension is $h^0(C,\sum z_j-K_C-P)$. Thus the determinant vanishes along $\alpha^*\Theta_P$, including multiplicities by the same determinant-complex argument as in part (i). The quotient is a rational section

$$
r=\frac{s_P}{s_0}\quad\text{of}\quad \det E_{L_P}\otimes(\det E_L)^{-1}\cong\bigotimes_{j=1}^n\operatorname{pr}_j^*P,
$$

with zero-minus-pole [Cartier divisor](../../../../../../cartier-divisor-split.md) $\alpha^*(\Theta_P-\Theta)$. The diagonal factors in the two determinants cancel.

Choose a trivialization $u:P^{\otimes N}\xrightarrow{\sim}\mathcal O_C$. This is possible because $P\in A[N]$. Taking the $N$th tensor power of $r$ and using $\bigotimes_j\operatorname{pr}_j^*u$ produces a scalar [rational function](../../../../../../rational-function.md) $R$ on $C^n$ with

$$
\operatorname{div}(R)=N\alpha^*\Theta_P-N\alpha^*\Theta.
$$

On $X$, the [Theorem of the square](../../../../../../theorem-of-the-square.md) and $NP=0$ imply

$$
\mathcal O_X(\Theta_P-\Theta)^{\otimes N}=\lambda(-P)^{\otimes N}\cong\mathcal O_X.
$$

Consequently there is a [rational function](../../../../../../rational-function.md) $f_P\in k(X)^\times$ with $\operatorname{div}(f_P)=N\Theta_P-N\Theta$. The map $\alpha$ is surjective, since every degree-$3g-3$ [line bundle](../../../../../../line-bundle.md) has a section by the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md). The two [rational functions](../../../../../../rational-function.md) $\alpha^*f_P$ and $R$ have the same [Cartier divisor](../../../../../../cartier-divisor-split.md) on the smooth projective connected product $C^n$; their quotient is an everywhere invertible regular function and hence a constant. Rescale $f_P$ to remove that constant. Away from the diagonals, ordinary evaluation gives

$$
\boxed{\alpha^*f_P=\left(\frac{\det(\sigma_i^P(z_j))}{\det(\sigma_i(z_j))}\right)^N,\qquad \operatorname{div}(f_P)=N\Theta_P-N\Theta,}
$$

where the $N$th power is interpreted with the chosen torsion trivialization. Equality as [rational functions](../../../../../../rational-function.md) then extends from this dense open set to the whole product.

The [torsion trivialization in a determinant quotient](../../../../../../torsion-trivialization-in-a-determinant-quotient.md) cannot be omitted if one uses raw meromorphic representatives. Explicitly, write $P=\mathcal O_C(p)$ and choose $h$ with $\operatorname{div}(h)=Np$. If $r_{\mathrm{raw}}$ is the quotient of the evaluation matrices in these meromorphic frames, then

$$
\operatorname{div}(r_{\mathrm{raw}})=\alpha^*(\Theta_P-\Theta)-\sum_j\operatorname{pr}_j^*p,\qquad R=r_{\mathrm{raw}}^N\prod_j h(z_j).
$$

Thus the displayed formula suppresses bundle trivializations; read as an unframed quotient of arbitrary meromorphic representatives, it needs precisely this extra product. Changes of bases or rescaling $u$ only change the allowable nonzero scalar normalization of $f_P$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
