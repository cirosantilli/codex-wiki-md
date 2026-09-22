<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $z=\lambda_z>0$. In cylindrical orthonormal bases the [principal stretches](../../../../../principal-stretch.md) are $r_{,R}$, $r/R$ and $z$. [Incompressibility](../../../../../incompressible-flow.md) gives

$$
r_{,R}\frac rR z=1,\qquad
\frac{d(r^2)}{dR}=\frac{2R}{z}.
$$

Integrate from the inner surface to obtain the [inflation and extension of an incompressible tube](../../../../../inflation-and-extension-of-an-incompressible-tube.md) kinematics

$$
r^2=a^2+\frac{R^2-a_0^2}{z},\qquad
\boxed{\lambda=\frac rR=z^{-1/2}
\left(1+\frac{za^2-a_0^2}{R^2}\right)^{1/2}.}
$$

In particular $b^2=a^2+(b_0^2-a_0^2)/z$. The radial [principal stretch](../../../../../principal-stretch.md) is $1/(z\lambda)$, so the reference-volume [strain energy density](../../../../../strain-energy-density.md) is $\widehat W(\lambda,z)$ with the three arguments $(1/(z\lambda),\lambda,z)$.

For reference length $L_0$, the stored energy is $L_0\mathcal E$, where

$$
\mathcal E(a,z)=2\pi\int_{a_0}^{b_0}\widehat W(\lambda(R;a,z),z)R\,dR.
$$

Let $N_{\rm wall}$ denote the total axial resultant acting on the material annulus. The work of the inner [pressure](../../../../../pressure.md) on the cylindrical wall is $2\pi azL_0p\dot a$, and axial work is $N_{\rm wall}L_0\dot z$. Reversible [virtual work](../../../../../virtual-work.md) therefore says

$$
2\pi azp\dot a+N_{\rm wall}\dot z
=\mathcal E_{,a}\dot a+\mathcal E_{,z}\dot z.
$$

The independent derivatives of the circumferential stretch are

$$
\lambda_{,a}=\frac{a}{\lambda R^2},\qquad
\left.\lambda_{,z}\right|_a
=-\frac{R^2-a_0^2}{2\lambda z^2R^2}.
$$

Equating the coefficients of $\dot a$ and $\dot z$ proves

$$
\boxed{p=\frac1z\int_{a_0}^{b_0}
\widehat W_{,\lambda}\frac{dR}{\lambda R},}
$$

and the corresponding axial resultant is

$$
\boxed{N_{\rm wall}=2\pi\int_{a_0}^{b_0}
\left[\widehat W_{,z}R
-\widehat W_{,\lambda}\frac{R^2-a_0^2}{2\lambda z^2R}\right]dR.}
$$

Here $\widehat W_{,z}$ holds $\lambda$ fixed. If $N$ means the independently applied load on pressurized closed ends, the [pressure](../../../../../pressure.md) also does axial end-cap work $\pi a^2pL_0\dot z$. Equivalently its complete work is $p\,d(\pi a^2zL_0)/dt$. In that convention,

$$
\boxed{N=N_{\rm wall}-\pi a^2p.}
$$

If $N$ includes the end-pressure resultant, it is $N_{\rm wall}$ itself. Stating this distinction is necessary because the ends are not specified; the [pressure](../../../../../pressure.md) formula is the same in both conventions.

For the specified [Mooney-Rivlin solid](../../../../../mooney-rivlin-solid.md) convention, differentiating the constrained [strain energy density](../../../../../strain-energy-density.md) gives

$$
\widehat W_{,\lambda}
=(\mu_1-\mu_2z^2)(\lambda-z^{-2}\lambda^{-3}).
$$

Thus

$$
p=z^{-1}(\mu_1-\mu_2z^2)
\int_{a_0}^{b_0}(1-z^{-2}\lambda^{-4})\frac{dR}{R}.
$$

Put $c=za^2-a_0^2$. If $c\ne0$, $z\lambda^2-1=c/R^2$ yields $dR/R=-z\lambda\,d\lambda/(z\lambda^2-1)$. The factor cancels because

$$
\frac{\lambda(1-z^{-2}\lambda^{-4})}{z\lambda^2-1}
=\frac1{z\lambda}+\frac1{z^2\lambda^3}.
$$

The limits are $\lambda_a=a/a_0$ and $\lambda_b=b/b_0$, so direct integration gives

$$
\boxed{p=(\mu_1z^{-2}-\mu_2)
\left[z\log\frac{\lambda_a}{\lambda_b}
-\frac12(\lambda_a^{-2}-\lambda_b^{-2})\right].}
$$

For $c=0$, all circumferential stretches equal $z^{-1/2}$ and the original integrand vanishes, so this formula still holds, with $p=0$. This also verifies its continuous limiting value without dividing by zero.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
