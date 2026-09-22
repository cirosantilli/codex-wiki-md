<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [natural units](../../../../../natural-units.md) with $c=1$, write $H=\dot a/a$, and measure [cosmic time](../../../../../cosmic-time.md) from the [Big Bang](../../../../../big-bang.md). The [cosmological continuity equation](../../../../../cosmological-continuity-equation.md) follows by differentiating the [Friedmann equation](../../../../../friedmann-equations.md) and using the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md); for [pressureless matter](../../../../../pressureless-matter.md) it gives $\dot\rho+3H\rho=0$, hence $\rho=\rho_0a^{-3}$ when the present [scale factor](../../../../../scale-factor-cosmology.md) is $a_0=1$. The present [critical density](../../../../../critical-density.md) and [cosmological density parameter](../../../../../cosmological-density-parameter.md) give

$$
\rho_{c0}=\frac{3H_0^2}{8\pi G},\qquad \rho_0=\Omega_0\rho_{c0},\qquad k=H_0^2(\Omega_0-1)>0.
$$

Consequently, with $C=H_0^2\Omega_0$, the [Friedmann equation](../../../../../friedmann-equations.md) becomes $\dot a^2=C/a-k$.

Introduce [conformal time](../../../../../conformal-time.md) through $dt=a\,d\tau$. A prime denotes a [derivative](../../../../../derivative.md) with respect to $\tau$, so $a'=a\dot a$ and

$$
(a')^2=Ca-ka^2=k\left[\left(\frac C{2k}\right)^2-\left(a-\frac C{2k}\right)^2\right].
$$

Set $u=\sqrt{k}\tau$, with $u=0$ at the [Big Bang](../../../../../big-bang.md). On the expanding branch the substitution $a=C(1-\cos u)/(2k)$ satisfies this equation. Integrating $dt=a\,du/\sqrt{k}$, with $t(0)=0$, gives the [closed matter-dominated Friedmann solution](../../../../../closed-matter-dominated-friedmann-solution.md):

$$
\boxed{a(\tau)=\frac{\Omega_0}{2(\Omega_0-1)}(1-\cos u),\qquad t(\tau)=\frac{\Omega_0}{2H_0(\Omega_0-1)^{3/2}}(u-\sin u),\qquad u=\sqrt{k}\tau.}
$$

The parametrization continues smoothly through the maximum [scale factor](../../../../../scale-factor-cosmology.md), reached at $u=\pi$, onto the contracting branch. Its curve in the $(t,a)$ plane is a rescaled [cycloid](../../../../../cycloid.md).

For a presently expanding universe, $H_0>0$ selects $0<u_0<\pi$. The normalization $a(u_0)=1$ gives

$$
\cos u_0=\frac2{\Omega_0}-1,\qquad \sin u_0=\frac{2\sqrt{\Omega_0-1}}{\Omega_0},\qquad u_0=\arccos\left(\frac2{\Omega_0}-1\right).
$$

Substitution yields the [age of a closed dust universe](../../../../../age-of-a-closed-dust-universe.md):

$$
\boxed{t_0=\frac{\Omega_0}{2H_0(\Omega_0-1)^{3/2}}\left[\arccos\left(\frac2{\Omega_0}-1\right)-\frac{2\sqrt{\Omega_0-1}}{\Omega_0}\right].}
$$

The first later zero of the [scale factor](../../../../../scale-factor-cosmology.md) occurs at $u=2\pi$, so the [lifetime of a closed dust universe](../../../../../lifetime-of-a-closed-dust-universe.md) gives the [Big Crunch](../../../../../big-crunch.md) time

$$
\boxed{t_{\rm BC}=\frac{\pi\Omega_0}{H_0(\Omega_0-1)^{3/2}}.}
$$

This is the total lifetime measured from the [Big Bang](../../../../../big-bang.md); the remaining [cosmic time](../../../../../cosmic-time.md) is $t_{\rm BC}-t_0$. As a check, the [limit](../../../../../limit-of-a-function.md) $\Omega_0\downarrow1$ gives $H_0t_0\to2/3$, while the [Big Crunch](../../../../../big-crunch.md) recedes to infinite time, as expected for a flat [matter-dominated universe](../../../../../matter-domination.md) with zero [cosmological constant](../../../../../cosmological-constant.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
