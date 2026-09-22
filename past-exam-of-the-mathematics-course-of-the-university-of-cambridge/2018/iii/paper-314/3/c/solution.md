<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For local cold [magnetocentrifugal acceleration](../../../../../../magnetocentrifugal-acceleration.md), the field must guide the gas and enforce approximate corotation with its disk footpoint in the sub-Alfvénic launching region. Let that footpoint be $R=R_f$, and keep its [field-line angular velocity](../../../../../../field-line-angular-velocity.md) $\Omega_f=\Omega(R_f)$ constant along the field. In this rotating frame the relevant [effective potential](../../../../../../effective-potential.md) is

$$
V(R,z)=\Phi(R,z)-\frac12\Omega_f^2R^2.
$$

The footpoint is a critical point because $\partial_R\Phi(R_f,0)=R_f\Omega_f^2$ and $\partial_z\Phi(R_f,0)=0$. The meridional [Hessian matrix](../../../../../../hessian-matrix.md) there is

$$
V_{RR}=-(\beta+2)\Omega_f^2,\qquad V_{zz}=\lambda^2\Omega_f^2,\qquad V_{Rz}=0.
$$

Take distance $\ell$ along a smooth outward [magnetic field line](../../../../../../magnetic-field-line.md) whose initial tangent is $(\sin\alpha,\cos\alpha)$ in the $(R,z)$ plane. Since the gradient of $V$ vanishes at the footpoint, field-line curvature does not contribute to its second derivative. Consequently

$$
V(\ell)-V(0)=\frac12\Omega_f^2\left[\lambda^2\cos^2\alpha-(\beta+2)\sin^2\alpha\right]\ell^2+O(\ell^3).
$$

A negative quadratic coefficient gives a downhill displacement and acceleration without thermal assistance. The [magnetocentrifugal launching criterion in a flattened power-law potential](../../../../../../magnetocentrifugal-launching-criterion-in-a-flattened-power-law-potential.md) is therefore

$$
\boxed{\tan^2\alpha>\frac{\lambda^2}{\beta+2},\qquad\alpha>\alpha_{\rm crit}=\arctan\left(\frac{|\lambda|}{\sqrt{\beta+2}}\right).}
$$

Angles are measured from the vertical, with $0\leq\alpha<\pi/2$. Below the critical angle the footpoint is a local minimum along the field, so a cold particle cannot cross the initial potential barrier. At equality the quadratic test is marginal; higher derivatives and the unspecified field curvature can decide the outcome. The threshold is a local condition for launch, not proof that the wind escapes along an arbitrary global field geometry. The spherical point-mass limit $\lambda=1$, $\beta\to1$ recovers $\alpha_{\rm crit}=30^\circ$, consistent with [Ogilvie's discussion of cold disk winds, section 9.9](https://arxiv.org/pdf/1604.03835).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
