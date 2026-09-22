<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Cooling from above makes dense cold fluid overlie lighter warm fluid, so the upper boundary layer is unstable and can mix the interior. Assume high [Rayleigh number](../../../../../../rayleigh-number.md), rapid interior mixing, constant properties, negligible wall heat capacity and a quasi-steady cooling flux obeying the [four-thirds convective heat-transfer law](../../../../../../four-thirds-convective-heat-transfer-law.md). Write $\theta(t)=T_{\rm bulk}(t)-T_0$ and use a coefficient $C$ appropriate to this single cooling boundary. The volumetric heat capacity is $\rho c_p=k/\kappa$, so the area-wise heat balance is

$$
\frac{kh}{\kappa}\dot\theta=-Ck\left(\frac{g\beta}{\nu\kappa}\right)^{1/3}\theta^{4/3}.
$$

With $K=C\kappa[g\beta/(\nu\kappa)]^{1/3}/h$, integration gives [convective cooling under the four-thirds heat-transfer law](../../../../../../convective-cooling-under-the-four-thirds-heat-transfer-law.md):

$$
\boxed{T_{\rm bulk}(t)=T_0+\left[(\Delta T)^{-1/3}+\frac K3t\right]^{-3}
=T_0+\Delta T\left[1+\frac{K(\Delta T)^{1/3}t}{3}\right]^{-3}.}
$$

The power-law decay is a bulk approximation between the initial boundary transient and the later stage when the decreasing temperature contrast no longer maintains strong convection. It is not an exact spatially uniform solution satisfying the cold boundary itself.

Cooling from below is different: dense cold fluid now lies below warm fluid and stabilizes the layer. With no other imposed motion, cooling is by [thermal conduction](../../../../../../thermal-conduction.md), and temperature becomes depth dependent. Let $z=0$ be the cooled bottom and $z=h$ the insulating top. Solve $\theta_t=\kappa\theta_{zz}$ with $\theta(0,t)=0$, $\theta_z(h,t)=0$ and $\theta(z,0)=\Delta T$. The mixed-boundary eigenfunctions have $\lambda_n=(n+1/2)\pi/h$, giving

$$
\boxed{T(z,t)-T_0=\frac{2\Delta T}{h}\sum_{n=0}^\infty
\frac{\sin(\lambda_nz)}{\lambda_n}e^{-\kappa\lambda_n^2t}.}
$$

Its volume-averaged temperature is

$$
\boxed{\overline T(t)-T_0=\frac{8\Delta T}{\pi^2}\sum_{n=0}^\infty
\frac{e^{-\kappa(2n+1)^2\pi^2t/(4h^2)}}{(2n+1)^2}.}
$$

The late conductive decay is exponential on the timescale $4h^2/(\pi^2\kappa)$, rather than the convective $t^{-3}$ bulk law. This assumes the usual positive thermal expansion coefficient and no destabilizing compositional stratification.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
