<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [stress-energy tensor](../../../../../../stress-energy-tensor.md) is already first order, so its energy flux can be evaluated on the unperturbed [Schwarzschild event horizon](../../../../../../schwarzschild-event-horizon.md) $r=2M_0$, with the infinity-normalized [Killing vector field](../../../../../../killing-vector-field.md) $\xi=\partial_v$. On this background $g^{rv}=1$, and hence

$$
T^r{}_b\xi^b=T^r{}_v=T_{vv}=\frac{\dot\mu}{4\pi(2M_0)^2}.
$$

The conserved [stress-energy current from a Killing vector](../../../../../../stress-energy-current-from-a-killing-vector.md) is $J^a=-T^a{}_b\xi^b$. Its radial component is negative, so the positive inward energy flux is $-J^r$. Using the directed null-surface measure $r_H^2\,dv\,d\Omega$ gives

$$
\Delta E=\int_{-\infty}^{\infty}\int_{S^2}T^r{}_v(2M_0)^2\,d\Omega\,dv
=\int_{-\infty}^{\infty}\dot\mu(v)\,dv
=\boxed{\Delta M}.
$$

The initial and final [event horizon](../../../../../../event-horizon.md) areas are $A_0=16\pi M_0^2$ and $A_1=16\pi(M_0+\Delta M)^2$. Thus $\Delta A=32\pi M_0\Delta M+O((\Delta M)^2)$. With [Schwarzschild surface gravity](../../../../../../schwarzschild-surface-gravity.md) $\kappa_0=1/(4M_0)$, the [Physical-process first law of black-hole mechanics](../../../../../../physical-process-first-law-of-black-hole-mechanics.md) follows:

$$
\boxed{\Delta E=\Delta M=\frac{\kappa_0}{8\pi}\Delta A+O((\Delta M)^2/M_0).}
$$

The flux is [Killing energy](../../../../../../killing-energy.md), including gravitational redshift, rather than the energy measured by a sequence of static observers arbitrarily close to the [event horizon](../../../../../../event-horizon.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
