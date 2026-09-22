<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [natural units](../../../../../natural-units.md) and [conformal time](../../../../../conformal-time.md) $dt=a\,d\tau$. The [conformal Hubble parameter](../../../../../conformal-hubble-parameter.md) is $\mathcal H=a'/a=aH$. For the [barotropic equation of state](../../../../../barotropic-equation-of-state.md) $P=(\gamma-1)\rho$, the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md) gives

$$
\mathcal H'=a\ddot a=-\frac{4\pi G}{3}a^2(3\gamma-2)\rho.
$$

The [Friedmann equation](../../../../../friedmann-equations.md) gives $8\pi Ga^2\rho/3=\mathcal H^2+k$. Hence the [constant-equation-of-state conformal Riccati equation](../../../../../constant-equation-of-state-conformal-riccati-equation.md) is

$$
\boxed{\mathcal H'+\alpha(\mathcal H^2+k)=0,\qquad\alpha=\frac{3\gamma-2}{2}.}
$$

For $\alpha\ne0$, separation and integration of this [Riccati equation](../../../../../riccati-equation.md) yield, after choosing the origin of [conformal time](../../../../../conformal-time.md),

$$
\boxed{\mathcal H=\begin{cases}
\cot(\alpha\tau),&k=1,\\
1/(\alpha\tau),&k=0,\\
\coth(\alpha\tau),&k=-1.
\end{cases}}
$$

The open positive-[energy density](../../../../../energy-density.md) branch uses the [hyperbolic cotangent](../../../../../hyperbolic-cotangent.md), rather than the [cotangent](../../../../../cotangent.md). Integrating $a'/a=\mathcal H$ gives

$$
\boxed{a(\tau)=\begin{cases}
A_+\sin^{1/\alpha}(\alpha\tau),&k=1,\\
A_0(\alpha\tau)^{1/\alpha},&k=0,\\
A_-\sinh^{1/\alpha}(\alpha\tau),&k=-1,
\end{cases}}
$$

where the positive constants are fixed by the [energy density](../../../../../energy-density.md) normalization. These formulas apply on branches where the bases are positive. For $\alpha>0$, take the [Big Bang](../../../../../big-bang.md) at $\tau=0$. The [cosmic time](../../../../../cosmic-time.md) is then

$$
t_+(\tau)=\frac{A_+}{\alpha}\int_0^{\alpha\tau}(\sin u)^{1/\alpha}\,du,\qquad
t_-(\tau)=\frac{A_-}{\alpha}\int_0^{\alpha\tau}(\sinh u)^{1/\alpha}\,du,
\qquad
t_0(\tau)=\frac{A_0}{\alpha+1}(\alpha\tau)^{(\alpha+1)/\alpha}.
$$

The [integrals](../../../../../integral.md) also give the general answer after selecting a suitable reference time when a finite [Big Bang](../../../../../big-bang.md) endpoint does not exist. The exceptional [coasting fluid](../../../../../coasting-fluid.md) $\gamma=2/3$ has $\alpha=0$, so $\mathcal H=h$ is constant: $a=Ae^{h\tau}$ and $t=(A/h)e^{h\tau}+t_*$. If $h=0$, instead $a=A$ and $t=A\tau+t_*$. A flat fluid with $\gamma=0$ is the constant-density [de Sitter spacetime](../../../../../de-sitter-spacetime.md) case, for which the flat time integral is logarithmic.

During [matter domination](../../../../../matter-domination.md), $\gamma=1$ and $\alpha=1/2$. Absorbing numerical factors into separate positive constants gives the [closed matter-dominated Friedmann solution](../../../../../closed-matter-dominated-friedmann-solution.md), the flat [Einstein-de Sitter universe](../../../../../einstein-de-sitter-universe.md) and the [open matter-dominated Friedmann solution](../../../../../open-matter-dominated-friedmann-solution.md):

$$
\begin{array}{c|c|c}
k&a(\tau)&t(\tau)\\\hline
1&C_+(1-\cos\tau)&C_+(\tau-\sin\tau)\\
0&C_0\tau^2&C_0\tau^3/3\\
-1&C_-(\cosh\tau-1)&C_-(\sinh\tau-\tau).
\end{array}
$$

To compare the [age of a dust universe without a cosmological constant](../../../../../age-of-a-dust-universe-without-a-cosmological-constant.md), specify the normalization. At fixed present [Hubble parameter](../../../../../hubble-parameter.md) $H_0$, with $x=a/a_0$ and present matter [cosmological density parameter](../../../../../cosmological-density-parameter.md) $\Omega_m>0$, the [Friedmann equation](../../../../../friedmann-equations.md) gives

$$
H_0t_0=\int_0^1\frac{\sqrt{x}\,dx}{\sqrt{\Omega_m+(1-\Omega_m)x}}.
$$

The integrand decreases strictly with $\Omega_m$ for $0<x<1$. Therefore [age ordering of dust universes at fixed Hubble parameter](../../../../../age-ordering-of-dust-universes-at-fixed-hubble-parameter.md) gives, on the expanding branches,

$$
\boxed{t_{\rm closed}<\frac{2}{3H_0}<t_{\rm open}<\frac1{H_0}.}
$$

The final bound is approached by the empty [Milne universe](../../../../../milne-model.md). This compares models with the same $H_0$; fixing instead the present [scale factor](../../../../../scale-factor-cosmology.md) and [energy density](../../../../../energy-density.md) gives a different comparison.

<a id="1/image-age-of-an-expanding-dust-universe-at-fixed-present-hubble-parameter"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-55-dust-age.png)

**[Figure 1](#1/image-age-of-an-expanding-dust-universe-at-fixed-present-hubble-parameter). Age of an expanding dust universe at fixed present Hubble parameter**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
