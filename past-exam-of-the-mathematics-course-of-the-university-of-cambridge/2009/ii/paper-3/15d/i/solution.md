<h1 id="15d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Mass conservation in the [Zeldovich approximation](../../../../../../zeldovich-approximation.md) gives $\rho\,d^3r=\bar\rho a^3\,d^3q$. Expanding the trajectory [Jacobian determinant](../../../../../../jacobian-determinant.md) to first order therefore yields $\boxed{\delta=-\nabla_q\cdot\Psi}$. At the same order, $\nabla_r=a^{-1}\nabla_q$ and

$$
\nabla_rP=c_s^2\nabla_r\rho=-\frac{\bar\rho c_s^2}{a}\nabla_q(\nabla_q\cdot\Psi)=-\frac{\bar\rho c_s^2}{a}\nabla_q^2\Psi.
$$

The last equality uses $\nabla_q\times\Psi=0$ and the [vector calculus](../../../../../../vector-calculus.md) $\nabla\operatorname{div}=\nabla^2+\nabla\times\nabla\times$.

Split the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) into its homogeneous-background and perturbed parts. The background has $\nabla_r\Phi_0=(4\pi G\bar\rho/3)r$. For the perturbation, [Poisson equation](../../../../../../poisson-equation.md) and irrotationality give

$$
\nabla_r\phi=-4\pi G\bar\rho\,a\Psi,
$$

with a harmonic or uniform-acceleration contribution set to zero by the perturbation boundary conditions. Its divergence is $-4\pi G\bar\rho\nabla_q\cdot\Psi=4\pi G\bar\rho\delta$, as required. Insert this and the pressure gradient into $\ddot r=\ddot a(q+\Psi)+2\dot a\dot\Psi+a\ddot\Psi$. The background acceleration cancels using $\ddot a/a=-4\pi G\bar\rho/3$, leaving

$$
\boxed{\ddot\Psi+2\frac{\dot a}{a}\dot\Psi-4\pi G\bar\rho\Psi-\frac{c_s^2}{a^2}\nabla_q^2\Psi=0.}
$$

Take minus the comoving divergence, and expand $\delta(q,t)=\sum_k\delta_k(t)e^{ik\cdot q}$. Since $\nabla_q^2$ acts on a [Fourier mode](../../../../../../fourier-mode.md) by $-k^2$, each mode satisfies

$$
\boxed{\ddot\delta_k+2\frac{\dot a}{a}\dot\delta_k-\left(4\pi G\bar\rho-\frac{c_s^2k^2}{a^2}\right)\delta_k=0.}
$$

Here the expansion coordinate is comoving; confusing it with the physical coordinate would lose the factor $a^{-2}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
