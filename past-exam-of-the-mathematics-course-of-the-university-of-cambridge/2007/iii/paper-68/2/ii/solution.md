<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Keep the background [magnetic field](../../../../../../magnetic-field.md), thermal gradient and [wavevector](../../../../../../wavevector.md) fixed as $|\Omega|\to\infty$. In particular, $k_z/K$ is nonzero and of order one. Put $H=g\alpha\beta$ and $X=\omega^2$. Multiplying the nonzero-frequency [dispersion relation](../../../../../../dispersion-relation.md) by $\omega^2$ gives

$$
K^2(X-a^2)^2-4\Omega^2k_z^2X+Hh^2(X-a^2)=0,
$$

that is,

$$
K^2X^2-\left(4\Omega^2k_z^2+2K^2a^2-Hh^2\right)X
+a^2(K^2a^2-Hh^2)=0.
$$

The sum and product of its two roots are

$$
X_f+X_s=\frac{4\Omega^2k_z^2}{K^2}+2a^2-\frac{Hh^2}{K^2},\qquad
X_fX_s=\frac{a^2(K^2a^2-Hh^2)}{K^2}.
$$

For large [rotation](../../../../../../rotation-mathematics.md), the sum is of order $\Omega^2$ while the product is independent of $\Omega$. The quadratic therefore has one large root and one small root. More explicitly,

$$
X_f=\frac{4\Omega^2k_z^2}{K^2}+O(1),\qquad
X_s=\frac{a^2(K^2a^2-Hh^2)}{4\Omega^2k_z^2}+O(|\Omega|^{-4}).
$$

The fast frequencies are consequently

$$
\boxed{\omega_f\sim\pm\frac{2|\Omega k_z|}{K}},
$$

which are [inertial waves](../../../../../../inertial-wave.md) at leading order. For nonzero $a$ away from the zero-frequency boundary, the [rapid-rotation slow magneto-Coriolis branch](../../../../../../rapid-rotation-slow-magneto-coriolis-branch.md) has

$$
\boxed{\omega_s\sim\pm\frac{|a|}{2|\Omega k_z|}\sqrt{K^2a^2-Hh^2}}.
$$

Its frequency is of order $|\Omega|^{-1}$, much smaller than the fast [inertial wave](../../../../../../inertial-wave.md) frequency. [Coriolis force](../../../../../../coriolis-force.md) balances most of the magnetic and buoyant forces in this slow motion, with inertia supplying only a small correction.

For $a^2>0$, **the slow wave has real nonzero frequency when**

$$
\boxed{\frac{(\mathbf B\cdot\mathbf k)^2}{\mu_0\rho}
>g\alpha\beta\frac{k_x^2+k_y^2}{|\mathbf k|^2}}.
$$

Stable thermal stratification has $H<0$ and automatically satisfies this condition. With adverse stratification, $H>0$, sufficiently strong [magnetic tension](../../../../../../magnetic-tension.md) along the [wavevector](../../../../../../wavevector.md) is needed. If the inequality is reversed, $X_s<0$ and the slow branch has imaginary frequencies, including an exponentially growing mode. Equality gives a stationary limit, rather than a nonzero oscillation. If $\mathbf B\cdot\mathbf k=0$, the proposed slow wave degenerates into zero-frequency disturbances: there is no magnetic restoring coupling. The remaining nonzero branch has $\omega^2=(4\Omega^2k_z^2-Hh^2)/K^2$. These qualifications also explain why zero roots introduced by clearing denominators must not be interpreted as ordinary propagating waves.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
