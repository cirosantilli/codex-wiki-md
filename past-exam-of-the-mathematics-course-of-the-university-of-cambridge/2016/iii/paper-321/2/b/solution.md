<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Substitute the axisymmetric [Fourier mode](../../../../../../fourier-mode.md) into the linearized equations. With hats denoting amplitudes,

$$
\begin{aligned}
-i\omega\hat v_x-2\Omega\hat v_y&=-ik_xc^2\hat\delta,\\
-i\omega\hat v_y+\frac\Omega2\hat v_x&=0,\\
-i\omega\hat v_z&=-ik_zc^2\hat\delta,\\
\omega\hat\delta&=k_x\hat v_x+k_z\hat v_z.
\end{aligned}
$$

For a nondegenerate nonzero frequency, eliminate the azimuthal velocity and use

$$
(\omega^2-\Omega^2)\hat v_x=\omega k_xc^2\hat\delta,\qquad \omega\hat v_z=k_zc^2\hat\delta.
$$

Continuity then gives

$$
\omega^2(\omega^2-\Omega^2)=c^2\left[k_x^2\omega^2+k_z^2(\omega^2-\Omega^2)\right].
$$

Equivalently, taking the [determinant](../../../../../../determinant.md) of the original four amplitude equations avoids division by zero and gives the full [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{\omega^4-(\Omega^2+c^2k^2)\omega^2+\Omega^2c^2k_z^2=0,\qquad k^2=k_x^2+k_z^2.}
$$

The two squared frequencies are

$$
\omega_\pm^2=\frac12\left[\Omega^2+c^2k^2\pm\sqrt{(\Omega^2+c^2k^2)^2-4\Omega^2c^2k_z^2}\right].
$$

The [discriminant](../../../../../../discriminant.md) is $(\Omega^2-c^2k^2)^2+4\Omega^2c^2k_x^2\ge0$. For $c^2>0$, both squared frequencies are nonnegative. The high-frequency branch is predominantly acoustic and the low-frequency branch is an [inertial wave](../../../../../../inertial-wave.md). Zero-frequency limiting modes, including $k_z=0$, are retained by the determinant calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
