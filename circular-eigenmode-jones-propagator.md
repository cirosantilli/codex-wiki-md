# Circular-eigenmode Jones propagator

↑ **Parent:** [Jones matrix](jones-matrix.md)

For fixed circular [eigenvectors](eigenvector.md) $\mathbf u_\pm=(1,\mp i)^{\mathsf T}/\sqrt2$, let $P_\pm=\mathbf u_\pm\mathbf u_\pm^\dagger$. A uniform optical medium with amplitude propagation coefficients $\gamma^\pm$ has the displayed [Jones matrix](jones-matrix.md). Put $\gamma=(\gamma^++\gamma^-)/2$ and $\delta=(\gamma^+-\gamma^-)/2$. Then

$$
\mathcal J(z)=e^{-\gamma z}
\begin{pmatrix}\cosh(\delta z)&-i\sinh(\delta z)\\i\sinh(\delta z)&\cosh(\delta z)\end{pmatrix}
=e^{-Kz},\qquad K=\begin{pmatrix}\gamma&i\delta\\-i\delta&\gamma\end{pmatrix}.
$$

The sum of the two modal exponentials supplies a hyperbolic cosine, not its reciprocal. The [determinant](determinant.md) is $e^{-2\gamma z}$, and $\mathcal J(z_1+z_2)=\mathcal J(z_1)\mathcal J(z_2)$. Real modal coefficients give [circular dichroism](circular-dichroism.md); purely imaginary coefficients give lossless [circular birefringence](circular-birefringence.md). Complex modal labels do not have an intrinsic numerical ordering.

## ↑ Ancestors (6)

1. [Jones matrix](jones-matrix.md)
2. [Jones calculus](jones-calculus.md)
3. [Polarization (waves)](polarization-waves.md)
4. [Wave](wave-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
