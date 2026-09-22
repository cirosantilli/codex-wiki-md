<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Neglecting cell rotational inertia, the light and viscous [torque](../../../../../../torque.md) sum to zero. Therefore the angular [velocity](../../../../../../velocity.md) is $\boldsymbol\Omega=\boldsymbol\omega/2+(\mathbf p\times\mathbf L)/\alpha$. A material orientation evolves by $\dot{\mathbf p}=\boldsymbol\Omega\times\mathbf p$. The vector triple-product identity gives

$$
\boxed{\dot{\mathbf p}=\frac12\boldsymbol\omega\times\mathbf p+\frac{\mathbf L-(\mathbf p\cdot\mathbf L)\mathbf p}{\alpha}.}
$$

The last term is the projection of $\mathbf L/\alpha$ onto the tangent plane to the unit sphere. In particular, $\mathbf p\cdot\dot{\mathbf p}=0$, as required to preserve the unit orientation. It aligns the swimmer towards the light; the [vorticity](../../../../../../vorticity.md) rotates that orientation.

For [rotational diffusion](../../../../../../rotational-diffusion.md) coefficient $D_r$, the [phototactic orientation Fokker-Planck equation](../../../../../../phototactic-orientation-fokker-planck-equation.md) balances deterministic orientation drift with diffusion on the sphere. Its density is normalized with respect to solid angle, not $d\theta\,d\phi$. When $\varepsilon=0$, there is no azimuthal drift and the zero-current condition is $f_{0,\theta}=-\lambda\sin\theta f_0$. Thus $f_0=\eta e^{\lambda\cos\theta}$, and normalization gives

$$
1=2\pi\eta\int_0^\pi e^{\lambda\cos\theta}\sin\theta\,d\theta=4\pi\eta\frac{\sinh\lambda}{\lambda},\qquad \boxed{\eta=\frac{\lambda}{4\pi\sinh\lambda}.}
$$

The limiting density at $\lambda=0$ is $1/(4\pi)$.

To justify the angular dependence of the first correction, define the operators

$$
\mathcal A=\nabla_p^2+\lambda(\sin\theta\,\partial_\theta+2\cos\theta),\qquad \mathcal R=\sin\phi\,\partial_\theta+\cot\theta\cos\phi\,\partial_\phi.
$$

The steady [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) is $\mathcal Af=-\varepsilon\mathcal Rf$. Its regular expansion $f=f_0+\varepsilon f^{(1)}+O(\varepsilon^2)$ therefore gives

$$
\mathcal Af^{(1)}=-\mathcal Rf_0=\lambda\eta\sin\theta\,e^{\lambda\cos\theta}\sin\phi.
$$

The coefficients of $\mathcal A$ are independent of $\phi$, so each azimuthal Fourier harmonic is preserved. The forcing has only the sine harmonic with azimuthal number one. There can be no extra unforced harmonic in a smooth normalized first correction: writing a homogeneous solution as $f_0h$ gives $\mathcal A(f_0h)=\nabla_p\cdot(f_0\nabla_ph)$. Multiplication by $h$ and [integration by parts](../../../../../../integration-by-parts.md) on the sphere gives $\int f_0|\nabla_ph|^2d\Omega=0$, hence $h$ is constant. Normalization $\int f^{(1)}d\Omega=0$ removes that multiple of $f_0$. It follows that

$$
\boxed{f=\eta e^{\lambda\cos\theta}+\varepsilon\eta\sin\phi\,g(\theta)+O(\varepsilon^2).}
$$

No explicit calculation of $g$ is needed. Its dependence is on $\theta$ and the parameter $\lambda$, and its behavior at the poles must make the density smooth.

In the stated spherical coordinates, $\mathbf p=\cos\theta\,\mathbf e_x+\sin\theta\cos\phi\,\mathbf e_y+\sin\theta\sin\phi\,\mathbf e_z$. Azimuthal integration makes the leading $y,z$ components and the first-order $x,y$ corrections vanish. The surviving coefficients are

$$
K_0=2\pi\eta\int_0^\pi\cos\theta\,e^{\lambda\cos\theta}\sin\theta\,d\theta,\qquad K_1=\pi\eta\int_0^\pi g(\theta)\sin^2\theta\,d\theta.
$$

Thus the [small-vorticity phototactic orientation response](../../../../../../small-vorticity-phototactic-orientation-response.md) is

$$
\boxed{\langle\mathbf p\rangle=K_0\mathbf e_x+\varepsilon K_1\mathbf e_z+O(\varepsilon^2).}
$$

Both coefficients depend only on $\lambda$. In particular, $K_0$ is the [Langevin function](../../../../../../langevin-function.md) of $\lambda$ and is positive for positive light strength; its integral representation above suffices.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
