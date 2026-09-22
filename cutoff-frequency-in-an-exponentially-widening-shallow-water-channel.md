# Cutoff frequency in an exponentially widening shallow-water channel

↑ **Parent:** [Shallow water equations](shallow-water-equations.md)

In a quasi-one-dimensional inviscid channel with depth $H$ and width $b(x)=b_0e^{\mu x}$, the linear [shallow water equations](shallow-water-equations.md) are $\eta_t+(H/b)(bu)_x=0$ and $u_t+g\eta_x=0$. Combining them gives $\eta_{tt}=gH(\eta_{xx}+\mu\eta_x)$.

For a time dependence $e^{i\omega t}$, write the elevation amplitude as $N(x)=e^{-\mu x/2}V(x)$. The spatial equation becomes

$$
V''+\left(\frac{\omega^2}{gH}-\frac{\mu^2}4\right)V=0.
$$

There is a travelling spatial phase only when the bracket is positive, so the [cutoff frequency](cutoff-frequency.md) is $\omega_c=\mu\sqrt{gH}/2$. Above it, an outgoing wave has a phase proportional to $\omega t-kx$ and amplitude proportional to $e^{-\mu x/2}$; below it the spatial response is evanescent. Geometric widening introduces the cutoff even though a constant-width channel has the nondispersive speed $\sqrt{gH}$.

## ↑ Ancestors (4)

1. [Shallow water equations](shallow-water-equations.md)
2. [Mathematical physics](mathematical-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2009/k/k4/solution.md)
