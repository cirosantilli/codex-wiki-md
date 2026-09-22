<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the displacement-potential convention $u_x=\partial_x\phi-\partial_z\psi$, $u_z=\partial_z\phi+\partial_x\psi$ and harmonic dependence $e^{-i\omega t}$. Choosing the opposite sign for the shear potential changes its column sign but not the [P-SV directional impedance matrix](../../../../../../p-sv-directional-impedance-matrix.md). Write $p=k_\alpha>0$, $s=k_\beta>0$, $D=k^2+ps$, and $H=\rho\omega^2-2\mu k^2$. At a common point the forward potential [wave amplitudes](../../../../../../wave-amplitude.md) give

$$
\begin{pmatrix}v_x\\v_z\end{pmatrix}=\omega\begin{pmatrix}k&-s\\p&k\end{pmatrix}\begin{pmatrix}\phi_+\\\psi_+\end{pmatrix},\qquad \begin{pmatrix}\sigma_{xz}\\\sigma_{zz}\end{pmatrix}=\begin{pmatrix}-2\mu kp&H\\-H&-2\mu ks\end{pmatrix}\begin{pmatrix}\phi_+\\\psi_+\end{pmatrix}.
$$

The [traction](../../../../../../traction.md) formulas follow from $\sigma_{xz}=\mu(u_{x,z}+u_{z,x})$ and $\sigma_{zz}=\lambda\nabla\cdot\mathbf u+2\mu u_{z,z}$, using $(\lambda+2\mu)\omega^2/\alpha^2=\rho\omega^2$ and $\mu(s^2-k^2)=H$. The [velocity](../../../../../../velocity.md) [matrix](../../../../../../matrix.md) has [determinant](../../../../../../determinant.md) $\omega^2D>0$, so elimination gives the [P-SV directional impedance matrix](../../../../../../p-sv-directional-impedance-matrix.md)

$$
\boxed{Z_+=\frac1{\omega D}\begin{pmatrix}\rho\omega^2p&k(2\mu D-\rho\omega^2)\\-k(2\mu D-\rho\omega^2)&\rho\omega^2s\end{pmatrix},\qquad\mathbf t=-Z_+\mathbf v.}
$$

Its off-diagonal entries are real and antisymmetric. Therefore

$$
Z_++Z_+^\dagger=\frac{2\rho\omega}{D}\begin{pmatrix}p&0\\0&s\end{pmatrix}.
$$

With real-part phasors, the outward $z$ flux is $-\tfrac12\operatorname{Re}(\mathbf v^\dagger\mathbf t)$, so

$$
\boxed{\langle S_z\rangle_+=\frac14\mathbf v^\dagger(Z_++Z_+^\dagger)\mathbf v=\frac{\rho\omega}{2D}\left(p|v_x|^2+s|v_z|^2\right)>0}
$$

for every nonzero forward [displacement field](../../../../../../displacement-field-mechanics.md). [Mass density](../../../../../../density.md) and [angular frequency](../../../../../../angular-frequency.md) are essential to this flux coefficient; both appear correctly in the PDF.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
