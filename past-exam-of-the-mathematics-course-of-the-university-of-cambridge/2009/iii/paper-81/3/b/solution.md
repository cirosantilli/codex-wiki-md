<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the rotation convention of part (a), so the orientation drift is $B^{-1}(\mathbf e_3-p_3\mathbf p)-\Omega\mathbf e_2\times\mathbf p$. The steady [gyrotactic orientation Fokker-Planck equation](../../../../../../gyrotactic-orientation-fokker-planck-equation.md) on the unit sphere is

$$
\nabla_p\cdot\left[\left\{\frac1B(\mathbf e_3-p_3\mathbf p)-\Omega\mathbf e_2\times\mathbf p\right\}f-D_R\nabla_pf\right]=0,\qquad \int f\,d\Omega=1.
$$

Let $\eta=(B\Omega)^{-1}$, $\lambda=(BD_R)^{-1}$, and introduce the rotation generator $\mathcal A=(\mathbf e_2\times\mathbf p)\cdot\nabla_p$. Dividing by $\Omega$ gives

$$
-\mathcal Af+\eta\nabla_p\cdot[(\mathbf e_3-p_3\mathbf p)f]-\frac\eta\lambda\Delta_pf=0.
$$

The leading isotropic density is $f_0=1/(4\pi)$. At first order, writing $f=f_0+\eta f_1+\cdots$, rotational [diffusion](../../../../../../diffusion.md) makes no contribution because $\Delta_pf_0=0$. The tangential drift is the spherical gradient of $p_3$, whose divergence is $\Delta_pp_3=-2p_3$. Therefore

$$
\mathcal Af_1=-2f_0p_3.
$$

In the polar convention of the paper, $p_1=\sin\theta\cos\phi$, and $\mathcal Ap_1=p_3$. Thus, in the specified first-harmonic form,

$$
\boxed{f=\frac1{4\pi}-\frac1{2\pi B\Omega}\sin\theta\cos\phi+O((B\Omega)^{-2}),\qquad\alpha=-\frac1{2\pi}.}
$$

The correction integrates to zero, preserving normalization. The first correction has no dependence on $\lambda$ because the isotropic leading density has zero spherical Laplacian; $\lambda$ enters the next-order equations.

Spherical symmetry gives $\int p_ip_jd\Omega=4\pi\delta_{ij}/3$. Consequently the [rapid-rotation mean gyrotactic orientation](../../../../../../rapid-rotation-mean-gyrotactic-orientation.md) is

$$
\boxed{\langle\mathbf p\rangle=-\frac{2}{3B\Omega}\mathbf e_1+O((B\Omega)^{-2}).}
$$

It is this small horizontal swimming bias, rather than a mean vertical orientation at leading order, that enters the concentration equation of part (c).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
