<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In charge-free, current-free vacuum, [Maxwell's equations](../../../../maxwell-equations-split.md) are

$$
\nabla\cdot\mathbf E=0,\qquad \nabla\cdot\mathbf B=0,\qquad
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t},\qquad
\nabla\times\mathbf B=\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t}.
$$

Taking the [curl](../../../../curl.md) of the third equation and using the fourth, the [curl of the curl identity](../../../../curl-of-the-curl-identity.md), and the zero [divergence](../../../../divergence.md) of the [electric field](../../../../electric-field-split.md) gives

$$
\nabla^2\mathbf E=\mu_0\epsilon_0\frac{\partial^2\mathbf E}{\partial t^2}.
$$

The [magnetic flux density](../../../../magnetic-field-split.md) obeys the same [wave equation](../../../../wave-equation-split.md). For the [plane wave](../../../../plane-wave.md) factor $e^{i(\omega t-kx)}$, the spatial [Laplacian](../../../../laplacian.md) contributes $-k^2$ and the second time [derivative](../../../../derivative.md) contributes $-\omega^2$. Thus

$$
k^2=\mu_0\epsilon_0\omega^2,\qquad
\boxed{c=\frac{\omega}{k}=\frac1{\sqrt{\mu_0\epsilon_0}}}
$$

for propagation in the positive $x$ direction. The zero-[divergence](../../../../divergence.md) conditions require $E_{0x}=B_{0x}=0$, while the [curl](../../../../curl.md) equations require $\mathbf B_0=(k/\omega)\hat{\mathbf x}\times\mathbf E_0$. These conditions show that the proposed [plane waves](../../../../plane-wave.md) satisfy all four [Maxwell's equations](../../../../maxwell-equations-split.md), rather than only their derived [wave equations](../../../../wave-equation-split.md). Physical [electric fields](../../../../electric-field-split.md) and [magnetic fields](../../../../magnetic-field-split.md) are the [real parts](../../../../real-part.md) of the complex expressions.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
