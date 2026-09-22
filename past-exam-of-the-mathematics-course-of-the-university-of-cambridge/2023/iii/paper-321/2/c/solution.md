<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For zero forcing, the given equation for $v_y$ is

$$
\left(\frac{D^2}{Dt^2}+\kappa_r^2-v_s^2\nabla^2\right)v_y=0.
$$

Use the [shearing-wave ansatz](../../../../../../shearing-wave-ansatz.md)

$$
v_y=\Re\left\{\widetilde v(t)
e^{i[k_x(t)x+k_yy]}\right\}.
$$

The explicit $x$ dependence cancels from the [material derivative](../../../../../../material-derivative.md) when

$$
\boxed{\dot k_x=Sk_y,
\qquad k_x(t)=k_x(0)+Sk_yt}.
$$

The amplitude then obeys the time-dependent [harmonic oscillator](../../../../../../simple-harmonic-motion.md) equation

$$
\boxed{\ddot{\widetilde v}+g(t)\widetilde v=0,
\qquad
g(t)=\kappa_r^2+v_s^2[k_x(t)^2+k_y^2]}.
$$

This evolving [wavevector](../../../../../../wavevector.md) is the characteristic signature of a [shearing wave](../../../../../../shearing-wave.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
