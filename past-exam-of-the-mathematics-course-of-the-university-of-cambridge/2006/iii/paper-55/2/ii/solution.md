<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Express the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) in variables $(\mathbf x,q,\mathbf n,\tau)$ and divide the derivative along the photon ray by $d\tau/d\lambda$. Since $f_0(q)$ has no explicit position, direction or conformal-time dependence,

$$
0=\frac{\partial f_1}{\partial\tau}
+P^i\frac{\partial f_1}{\partial x^i}
+\frac{dq}{d\tau}\frac{df_0}{dq}
+\frac{dq}{d\tau}\frac{\partial f_1}{\partial q}
+\frac{dn^i}{d\tau}\frac{\partial f_1}{\partial n^i}.
$$

This is the chain rule in momentum magnitude and direction. At linear order, $P^i=n^i+O(h)$, while the last two terms are products of first-order perturbations and can be dropped. The [synchronous photon momentum redshift](../../../../../../synchronous-photon-momentum-redshift.md) from part i then gives, for spatial Fourier convention $e^{i\mathbf k\cdot\mathbf x}$,

$$
\boxed{f_1'+ik\mu f_1=\frac12q\frac{df_0}{dq}h'_{ij}n^in^j,\qquad
\mu=\widehat{\mathbf k}\cdot\mathbf n.}
$$

The factor $q$ is essential. It is missing in the PDF's displayed intermediate equation, but follows directly from part i and is needed to obtain its final brightness equation.

Let $I_0=\int_0^\infty q^3f_0(q)\,dq$. Absorbing the common phase-space normalization into $f$, the homogeneous photon energy density is $\rho_\gamma=4\pi I_0/a^4$, so the [photon brightness perturbation](../../../../../../photon-brightness-perturbation.md) is

$$
\Delta=\frac{\int_0^\infty q^3f_1\,dq}{I_0}.
$$

A small directional temperature change $\Theta=\Delta T/T$ in a [Planck distribution](../../../../../../planck-photon-distribution.md) gives $f_1=-qf_0'(q)\Theta$. Integration by parts yields

$$
\int_0^\infty q^4f_0'(q)\,dq
=\left[q^4f_0(q)\right]_0^\infty-4I_0=-4I_0,
$$

because the [Planck distribution](../../../../../../planck-photon-distribution.md) behaves as $q^{-1}$ at low momentum and decays exponentially at high momentum. Thus $\Delta=4\Theta$. Equivalently, frequency-integrated [blackbody radiation](../../../../../../black-body-radiation.md) energy scales as $T^4$. Identifying brightness with a single temperature perturbation assumes this [blackbody](../../../../../../blackbody.md) spectral form; the brightness integral itself is defined more generally.

Finally, multiply the corrected transport equation by $q^3$, integrate and divide by $I_0$. The spatial streaming factor is independent of $q$, while its gravitational source integrates to $(1/2)(-4)h'_{ij}n^in^j$. Therefore

$$
\boxed{\Delta'+ik\mu\Delta=-2h'_{ij}n^in^j.}
$$

This derives the [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md) with the normalization and sign fixed, rather than inferring it from the dimensionally inconsistent intermediate formula.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
