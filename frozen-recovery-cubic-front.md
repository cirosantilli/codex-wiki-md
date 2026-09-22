# Frozen-recovery cubic front

↑ **Parent:** [FitzHugh-Nagumo model](fitzhugh-nagumo-model.md)

For the scalar [reaction-diffusion equation](reaction-diffusion-system.md) $v_t=Dv_{xx}-(v-r_1)(v-r_2)(v-r_3)$ with $D>0$ and $r_1<r_2<r_3$, an exact decreasing [travelling wave](travelling-wave.md) is

$$
V(z)=r_1+\frac{r_3-r_1}{1+\exp[(r_3-r_1)(z-z_0)/\sqrt{2D}]},\qquad z=x-ct.
$$

Indeed $V'=-(V-r_1)(r_3-V)/\sqrt{2D}$, and substitution into $DV''+cV'-(V-r_1)(V-r_2)(V-r_3)=0$ leaves the factor $(r_1+r_3)/2-r_2-c/\sqrt{2D}$, proving the speed formula. A zero speed gives the [Maxwell balance for a scalar reaction-diffusion front](maxwell-balance-for-a-scalar-reaction-diffusion-front.md). In a [FitzHugh-Nagumo model](fitzhugh-nagumo-model.md) this calculation requires treating the [recovery variable](recovery-variable.md) as frozen externally: retaining $w_t=\beta v-\gamma w$ with exactly constant $w$ forces $v$ to be constant.

## ↑ Ancestors (5)

1. [FitzHugh-Nagumo model](fitzhugh-nagumo-model.md)
2. [Mathematical biology](mathematical-biology-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-further-mathematical-biology-course-of-the-university-of-oxford/2023/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford/2010/b/5/c/iii/solution.md)
