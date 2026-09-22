<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The accumulated [point charge](../../../../../../point-charge.md) $Q(t)$ produces

$$
\boxed{\mathbf E(r,t)
=\frac{Q(t)}{4\pi\epsilon_0r^2}\mathbf e_r}.
$$

Since $\dot Q=I$, the [displacement current](../../../../../../displacement-current.md) density is

$$
\boxed{\epsilon_0\frac{\partial\mathbf E}{\partial t}
=\frac{I}{4\pi r^2}\mathbf e_r}.
$$

Apply the integral [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) to the boundary of a [spherical cap](../../../../../../spherical-cap.md) of radius $r$ and polar angle $\theta<\pi/2$. By axial symmetry $\mathbf B=B_\phi\mathbf e_\phi$ is constant along the boundary, whose circumference is $2\pi r\sin\theta$. The displacement-current flux through the cap is

$$
\int_{\rm cap}\frac{I}{4\pi r^2}\,dA
=\frac{I}{4\pi r^2}\,2\pi r^2(1-\cos\theta)
=\frac I2(1-\cos\theta).
$$

Thus

$$
2\pi r\sin\theta\,B_\phi
=\frac{\mu_0I}{2}(1-\cos\theta).
$$

Using $(1-\cos\theta)/\sin\theta=\tan(\theta/2)$ gives

$$
\boxed{\mathbf B(r,\theta)
=\frac{\mu_0I}{4\pi r}
\tan\!\left(\frac\theta2\right)\mathbf e_\phi}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
