# Discrete gauge cancellation in two-path interference

↑ **Parent:** [Aharonov-Bohm effect](aharonov-bohm-effect.md)

A four-vertex model proves the essential [gauge invariance](gauge-invariance.md) without solving an [electron](electron.md) scattering problem. Use two directed paths $S\to U\to D$ and $S\to L\to D$. Assign an edge phase $a_{ij}$ and a complex unit link $U_{ij}=e^{ia_{ij}}$ to each directed edge, with $U_{ji}=U_{ij}^{-1}$. These links represent discretized magnetic [line integrals](line-integral.md) multiplied by $q/\hbar$. Under a [gauge transformation](gauge-transformation.md) with arbitrary vertex phases $\chi_i$,

$$
a'_{ij}=a_{ij}+\chi_j-\chi_i,\qquad
P_1=U_{SU}U_{UD},\qquad P_2=U_{SL}U_{LD}.
$$

Both path products acquire the same factor $e^{i(\chi_D-\chi_S)}$. Their [gauge-invariant](gauge-invariance.md) ratio is the closed-loop [holonomy](holonomy.md)

$$
W_C=P_1P_2^*=\exp\!\left(i[a_{SU}+a_{UD}-a_{SL}-a_{LD}]\right)=e^{i\delta}.
$$

Every intermediate vertex phase cancels. For any fixed nonnegative real amplitudes $a,b$, the [interference](interference-wave-propagation.md) quantity $|aP_1+bP_2|^2$ is unchanged too. A gauge-dependent open-path phase consequently cannot be interpreted as an observable by itself.

For an exact example, measure phases in units of $\pi$ and order edges as $(SU,UD,SL,LD)$. Choose edge phases $(0,0,0,1/2)$ and vertex phases $(\chi_S,\chi_U,\chi_L,\chi_D)=(1/3,-1/4,2/5,1/7)\pi$. The transformed edge phases are

$$
(a'_{SU},a'_{UD},a'_{SL},a'_{LD})
=\left(-\frac7{12},\frac{11}{28},\frac1{15},\frac{17}{70}\right)\pi.
$$

The upper and lower sums become $-4\pi/21$ and $13\pi/42$; their difference remains $-\pi/2$. With amplitudes $a=1$, $b=1/2$, the intensity remains $5/4$. Sweeping one physical loop phase through $2\pi$ instead produces extrema $9/4$ and $1/4$, agreeing with the [interferometric visibility](interferometric-visibility.md) example above.

<a id="image-flux-moves-fringes-while-vertex-gauge-phases-cancel"></a>
![](aharonov-bohm-flux-fringes-and-gauge-cancellation.png)

**[Figure 2](#image-flux-moves-fringes-while-vertex-gauge-phases-cancel). Flux moves fringes while vertex gauge phases cancel**. [Source](aharonov-bohm-flux-fringes-and-gauge-cancellation.py). Original scalar two-path calculation with $I_1=1$ and $I_2=1/4$. Left: carrier fringes at three chosen enclosed fluxes, in units of the [electron](electron.md) period $h/e$. Right: the exact four-edge example before and after a vertex [gauge transformation](gauge-transformation.md); open-path phase sums change together and their difference is fixed. Curves are illustrative model intensities, not an experimental interferogram.

## ↑ Ancestors (8)

1. [Aharonov-Bohm effect](aharonov-bohm-effect.md)
2. [Charge-flux composite](charge-flux-composite.md)
3. [Anyon](anyon.md)
4. [Topological quantum matter](topological-quantum-matter-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
