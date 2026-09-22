<h1 id="30e/solution">Solution</h1>

↑ **Parent:** [30E](../30e.md)

For the disc, put $u(r,\varphi)=R_0(r)\Theta(\varphi)$. The polar [Laplace equation](../../../../../laplace-equation.md) separates as

$$
\Theta''+n^2\Theta=0,\qquad
r^2R_0''+rR_0'-n^2R_0=0,
$$

where periodicity requires an integer $n\ge0$. The radial ansatz $R_0=r^\alpha$ gives $\alpha=\pm n$; for $n=0$ the solutions are a constant and $\log r$. Regularity at the origin excludes negative powers and the logarithm.

Writing the boundary data as a [Fourier series](../../../../../fourier-series-split.md)

$$
u_D(\varphi)=a_0+\sum_{n\ge1}(a_n\cos n\varphi+b_n\sin n\varphi),
$$

with $a_0=(2\pi)^{-1}\int_0^{2\pi}u_D$, $a_n=\pi^{-1}\int_0^{2\pi}u_D\cos n\varphi$, and the analogous formula for $b_n$, gives

$$
\boxed{u(r,\varphi)=a_0+
\sum_{n\ge1}(r/R)^n(a_n\cos n\varphi+b_n\sin n\varphi).}
$$

Equivalently it is the [Poisson integral on the unit disk](../../../../../poisson-integral-on-the-unit-disk.md) with kernel

$$
\frac{R^2-r^2}{R^2-2Rr\cos(\varphi-\psi)+r^2}.
$$

For continuous boundary data this integral converges to the prescribed value at every boundary point, is smooth and harmonic inside, and uniqueness follows from the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md).

For the square, superpose four solutions, each carrying one side's data and zero data on the other three sides. Set $k_n=n\pi/a$ and

$$
f_{j,n}=\frac2a\int_0^af_j(s)\sin(k_ns)\,ds.
$$

[Separation of variables](../../../../../separation-of-variables.md) gives the explicit sum

$$
\boxed{\begin{aligned}
u(x,y)=\sum_{n\ge1}\frac1{\sinh(k_na)}
\big[&
f_{1,n}\sin(k_nx)\sinh(k_n(a-y))\\
+&f_{2,n}\sin(k_nx)\sinh(k_ny)\\
+&f_{3,n}\sin(k_ny)\sinh(k_n(a-x))\\
+&f_{4,n}\sin(k_ny)\sinh(k_nx)\big].
\end{aligned}}
$$

Each summand has zero Laplacian and the required zero values on three open sides. The [Fourier sine series](../../../../../fourier-sine-series.md) supplies the fourth side. For regular continuous data with matching values at the corners, the harmonic extension also takes the common corner values; termwise boundary evaluation of the sine series at the corners is not valid in general. For incompatible corner data there is no continuous solution on the closed square, but the displayed harmonic solution still attains the prescribed data on each open side.

## ↑ Ancestors (10)

1. [30E](../30e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
