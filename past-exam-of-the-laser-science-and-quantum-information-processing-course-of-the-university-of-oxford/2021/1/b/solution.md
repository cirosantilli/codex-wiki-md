<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [thin lens](../../../../thin-lens.md) has [ray transfer matrix](../../../../ray-transfer-matrix-analysis.md)

$$
M=\begin{pmatrix}1&0\\-1/f&1\end{pmatrix}.
$$

The [complex beam parameter](../../../../complex-beam-parameter.md) transformation gives $q_2=q_1/(1-q_1/f)$, hence

$$
\boxed{\frac1{q_1}-\frac1{q_2}=\frac1f.}
$$

The sign is also obtained by multiplying the incident [wave amplitude](../../../../wave-amplitude.md) by the [thin lens](../../../../thin-lens.md) [phase](../../../../phase-waves.md) $\exp[-ik\rho^2/(2f)]$.

Choose the [thin lens](../../../../thin-lens.md) plane as $z=0$ and put $a=\pi w_0^2/\lambda$, the incident [Rayleigh range](../../../../rayleigh-length.md). Since the incident [beam waist](../../../../beam-waist.md) lies there, $q_1=-ia$. Immediately after the [thin lens](../../../../thin-lens.md),

$$
q_2=\frac{-ia}{1+ia/f}
=-\frac{fa^2}{f^2+a^2}-i\frac{f^2a}{f^2+a^2}.
$$

Subsequent free propagation adds $z$, so write $q(z)=z-z_f-iz_R'$. Comparing real and imaginary parts gives

$$
\boxed{z_f=\frac{fa^2}{f^2+a^2},\qquad
z_R'=\frac{f^2a}{f^2+a^2},\qquad
w_f^2=\frac{\lambda z_R'}\pi.}
$$

For a positive [focal length](../../../../focal-length.md), the new [beam waist](../../../../beam-waist.md) lies downstream but closer than the geometrical focus. At fixed $f,\lambda$, as $w_0\to\infty$,

$$
\boxed{z_f\to f,\quad z_R'\sim\frac{f^2\lambda}{\pi w_0^2}\to0,
\quad w_f\sim\frac{f\lambda}{\pi w_0}.}
$$

This is the formal unbounded-[aperture](../../../../aperture.md) scalar limit; eventually finite [aperture](../../../../aperture.md) and the [paraxial approximation](../../../../paraxial-approximation.md) limit the extrapolation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
