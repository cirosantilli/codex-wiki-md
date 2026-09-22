<h1 id="38a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the real mode

$$
w=A\sin(q_ny)\cos(kx-\omega t).
$$

The [kinetic energy density](../../../../../../kinetic-energy-density.md) and [isotropic linear-elastic energy density](../../../../../../isotropic-linear-elastic-energy-density.md) are

$$
e_k=\frac12\rho w_t^2,
\qquad
e_p=\frac\mu2(w_x^2+w_y^2).
$$

Average over one period and integrate across the layer. Since $\int_0^h\sin^2(q_ny)\,dy=\int_0^h\cos^2(q_ny)\,dy=h/2$, the mean energy per unit horizontal area is

$$
\overline{\mathcal E}
=\int_0^h\overline{e_k+e_p}\,dy
=\frac{\rho A^2\omega^2h}{4}.
$$

The $x$-directed elastic-energy flux is $S_x=-\sigma_{zx}w_t=-\mu w_xw_t$. Its corresponding average is

$$
\overline{\mathcal F}_x
=\int_0^h\overline{S_x}\,dy
=\frac{\mu A^2k\omega h}{4}.
$$

Using $\omega^2=c_S^2(k^2+q_n^2)$ gives

$$
\frac{\overline{\mathcal F}_x}{\overline{\mathcal E}}
=\frac{\mu k}{\rho\omega}
=\frac{c_S^2k}{\omega}
=c_{g,n},
$$

and therefore

$$
\boxed{\overline{\mathcal F}_x=c_{g,n}\overline{\mathcal E}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [38A](../../38a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
