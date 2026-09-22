<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

Assume the particle [masses](../../../../../mass.md) $m_i$ are fixed and their total [mass](../../../../../mass.md) $M=\sum_i m_i$ is positive. The [centre of mass](../../../../../center-of-mass.md) and the relative [position](../../../../../position.md) vectors are

$$
\boxed{\mathbf R=\frac1M\sum_i m_i\mathbf x_i,\qquad\mathbf y_i=\mathbf x_i-\mathbf R.}
$$

Their weighted sum is zero, so [differentiation](../../../../../differentiation.md) gives $\sum_i m_i\dot{\mathbf y}_i=0$. Expanding the [kinetic energy](../../../../../kinetic-energy.md) with $\dot{\mathbf x}_i=\dot{\mathbf R}+\dot{\mathbf y}_i$ makes the mixed term vanish:

$$
T=\frac12\sum_i m_i\bigl(|\dot{\mathbf R}|^2+2\dot{\mathbf R}\cdot\dot{\mathbf y}_i+|\dot{\mathbf y}_i|^2\bigr)
=\boxed{\frac12M|\dot{\mathbf R}|^2+\frac12\sum_i m_i|\dot{\mathbf y}_i|^2}.
$$

This [kinetic-energy decomposition about the centre of mass](../../../../../kinetic-energy-decomposition-about-the-centre-of-mass.md) separates translation from internal motion without assuming any particular [force](../../../../../force.md) law.

For the [rigid body](../../../../../rigid-body-dynamics.md), its relative [velocity](../../../../../velocity.md) is $\dot{\mathbf y}_i=\omega\mathbf n\times\mathbf y_i$. The [cross product](../../../../../cross-product.md) identity for a [unit vector](../../../../../unit-vector.md) gives $|\mathbf n\times\mathbf y_i|^2=|\mathbf y_i|^2-(\mathbf n\cdot\mathbf y_i)^2$, the squared perpendicular distance to the rotation axis. Hence the [moment of inertia](../../../../../moment-of-inertia.md) of the particle is $I_i=m_i[|\mathbf y_i|^2-(\mathbf n\cdot\mathbf y_i)^2]$, and summing the [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) yields

$$
\boxed{T=\frac12M|\dot{\mathbf R}|^2+\frac12I\omega^2,\qquad I=\sum_i I_i.}
$$

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
