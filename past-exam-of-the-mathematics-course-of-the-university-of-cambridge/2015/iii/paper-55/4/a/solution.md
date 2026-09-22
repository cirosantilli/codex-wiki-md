<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [scalar cosmological perturbation](../../../../../../scalar-cosmological-perturbation.md) at fixed wavevector carries no helicity or distinguished transverse direction. Its metric and scalar sources are unchanged by rotations around $\mathbf k$, and the scalar baryon [peculiar velocity](../../../../../../peculiar-velocity.md) is longitudinal. With scalar initial conditions, rotational invariance of the linear evolution therefore makes $\Theta$ a function only of $\mu=\hat{\mathbf k}\cdot\mathbf e$. Expand it using the stated normalization, without an extra $(2\ell+1)$ factor:

$$
\Theta(\mu)=\sum_{\ell\ge0}(-i)^\ell\Theta_\ell P_\ell(\mu),\qquad
\Theta_\ell=i^\ell\frac{2\ell+1}2\int_{-1}^1d\mu\,P_\ell(\mu)\Theta(\mu).
$$

In the Thomson kernel, $1+v^2=4/3+(2/3)P_2(v)$. The [spherical harmonic addition theorem](../../../../../../spherical-harmonic-addition-theorem.md) and [Orthogonality of Legendre polynomials](../../../../../../orthogonality-of-legendre-polynomials.md) give

$$
\int\frac{d\hat{\mathbf m}}{4\pi}P_\ell(\hat{\mathbf k}\cdot\hat{\mathbf m})P_L(\mathbf e\cdot\hat{\mathbf m})
=\frac{\delta_{\ell L}}{2\ell+1}P_\ell(\hat{\mathbf k}\cdot\mathbf e).
$$

Only the monopole and quadrupole survive; the quadrupole's $(-i)^2=-1$ gives **the angular scattering integral**

$$
\boxed{\int\frac{d\hat{\mathbf m}}{4\pi}\Theta(\hat{\mathbf m})[1+(\mathbf e\cdot\hat{\mathbf m})^2]
=\frac43\Theta_0-\frac2{15}\Theta_2P_2(\mu).}
$$

This also explains why an isotropic distribution has zero net collision term.

The streaming term $ik\mu\Theta$ and the [Legendre polynomial recurrence relation](../../../../../../legendre-polynomial-recurrence-relation.md) yield, after division by $(-i)^\ell$, $k[(\ell+1)\Theta_{\ell+1}/(2\ell+3)-\ell\Theta_{\ell-1}/(2\ell-1)]$. With $\mathbf v_b=i\hat{\mathbf k}v_b$, the velocity collision source is $+\tau'v_b$ in the dipole equation; the gravitational gradient source is $+k\psi$. Therefore **the [photon Boltzmann hierarchy](../../../../../../photon-boltzmann-hierarchy.md) is**

$$
\boxed{\Theta_\ell'+k\left[\frac{\ell+1}{2\ell+3}\Theta_{\ell+1}-\frac\ell{2\ell-1}\Theta_{\ell-1}\right]
=\tau'\left[(1-\delta_{\ell0})\Theta_\ell+\delta_{\ell1}v_b-\frac1{10}\delta_{\ell2}\Theta_2\right]
+\delta_{\ell0}\phi'+\delta_{\ell1}k\psi.}
$$

Set the absent $\Theta_{-1}$ contribution to zero. This is algebraically the printed hierarchy. In particular,

$$
\Theta_0'+\frac k3\Theta_1=\phi',\quad
\Theta_1'+k\left(\frac25\Theta_2-\Theta_0\right)=\tau'(\Theta_1+v_b)+k\psi,
$$



$$
\Theta_2'+k\left(\frac37\Theta_3-\frac23\Theta_1\right)=\frac9{10}\tau'\Theta_2.
$$

Since $\tau'<0$, these collision terms damp the nonzero multipoles and drive the dipole to $\Theta_1=-v_b$. The latter sign follows from the paper's velocity and $(-i)^\ell$ conventions, not a reversed physical photon velocity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
