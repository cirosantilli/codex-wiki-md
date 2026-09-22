<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
\kappa=\frac{k}{\rho c_p},
\qquad
\kappa_s=\frac{k_s}{\rho c_p},
\qquad
h(t)=2\lambda\sqrt{\kappa t}.
$$

The [Neumann solution of the Stefan problem](../../../../../../neumann-solution-of-the-stefan-problem.md) in the ice and substrate is

$$
T_i(z,t)=T_0+(T_m-T_0)
\frac{\operatorname{erf}(z/(2\sqrt{\kappa t}))}
{\operatorname{erf}\lambda}
\quad(0<z<h),
$$

and

$$
T_s(z,t)=T_s+(T_0-T_s)
\operatorname{erfc}\left(\frac{-z}{2\sqrt{\kappa_st}}\right)
\quad(z<0).
$$

Continuity of [heat flux](../../../../../../heat-flux-density.md) at the contact gives, with $r=\sqrt{k_s/k}$,

$$
\frac{T_m-T_0}{\operatorname{erf}\lambda}
=r(T_0-T_s),
$$

and therefore

$$
\boxed{
T_0=\frac{T_m+r\operatorname{erf}(\lambda)T_s}
{1+r\operatorname{erf}(\lambda)}}.
$$

At the ice–water interface, the water is isothermal at $T_m$. The [Stefan condition](../../../../../../stefan-condition.md) $\rho L\dot h=kT_{i,z}(h^-)$ gives

$$
S\lambda
=\frac{T_m-T_0}{T_m-T_s}
\frac{e^{-\lambda^2}}
{\sqrt\pi\operatorname{erf}\lambda},
\qquad
S=\frac{L}{c_p(T_m-T_s)}.
$$

Eliminating $T_0$ yields the implicit equation

$$
\boxed{
\sqrt\pi S\lambda e^{\lambda^2}
\left(1+r\operatorname{erf}\lambda\right)=r},
$$

which determines $\lambda$ and hence $h(t)=2\lambda\sqrt{\kappa t}$.

If $k_s\gg k$, then $r\gg1$, $T_0\sim T_s$, and

$$
\boxed{S\lambda\sim
\frac{e^{-\lambda^2}}{\sqrt\pi\operatorname{erf}\lambda}}.
$$

The highly conducting substrate acts as a reservoir fixed near its initial cold temperature, giving the usual one-phase [Stefan problem](../../../../../../stefan-problem.md).

If $k_s\ll k$, then $r\ll1$, $T_0\sim T_m$, and $\lambda\sim r/(\sqrt\pi S)$. Consequently

$$
\boxed{
h(t)\sim\frac{2c_p(T_m-T_s)}{L}
\sqrt{\frac{\kappa_st}{\pi}}}.
$$

Here heat removal through the poorly conducting substrate is rate limiting, and only a small temperature drop is needed across the much more conducting ice.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
