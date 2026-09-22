<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $K^2=|\mathbf k|^2=k_x^2+k_z^2+\Omega^2t^2k_x^2$. For the complex wave before taking its [real part](../../../../../../real-part.md),

$$
(\partial_t+\Omega y\partial_x)(\mathbf v e^{i\mathbf k\cdot\mathbf x})=\left[\dot{\mathbf v}+i(\dot{\mathbf k}\cdot\mathbf x+\Omega yk_x)\mathbf v\right]e^{i\mathbf k\cdot\mathbf x}=\dot{\mathbf v}e^{i\mathbf k\cdot\mathbf x},
$$

since $\dot k_y=-\Omega k_x$. The asserted [velocity](../../../../../../velocity.md) equation therefore follows directly from $\dot{\mathbf v}+\Omega v_y\widehat{\mathbf x}=-i\mathbf kq$. To verify the [pressure](../../../../../../pressure.md) amplitude, solenoidality is $\mathbf k\cdot\mathbf v=0$. Its derivative requires

$$
0=\dot{\mathbf k}\cdot\mathbf v+\mathbf k\cdot\dot{\mathbf v}=-2\Omega k_xv_y-iK^2q,
$$

and hence $q=2i\Omega k_xv_y/K^2$, as claimed.

The transverse amplitude equations are

$$
\dot v_y=av_y,\qquad\dot v_z=bv_y,\qquad a=\frac{2\Omega k_xk_y}{K^2},\quad b=\frac{2\Omega k_xk_z}{K^2}.
$$

Both coefficients are real. Differentiating $v_yv_z^*-v_zv_y^*$ makes the terms proportional to $b|v_y|^2$ cancel, while the remaining terms give $a(v_yv_z^*-v_zv_y^*)$. Therefore the [helicity invariant of an inviscid shearing wave](../../../../../../helicity-invariant-of-an-inviscid-shearing-wave.md) obeys

$$
\boxed{\dot H=\frac{2\Omega k_xk_y}{K^2}H=-\frac{2\Omega^2tk_x^2}{k_x^2+k_z^2+\Omega^2t^2k_x^2}H,\qquad H(t)=\frac{H_0(k_x^2+k_z^2)}{k_x^2+k_z^2+\Omega^2t^2k_x^2}.}
$$

Here $H$ is real because the difference in its definition is purely imaginary. Its sign is preserved, and shear reduces its magnitude away from $t=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
