<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Specify the [spin](../../../../spin.md) counting first. Let $g_s=g_s(E_F)$ denote the unpolarized [single-spin density of states](../../../../single-spin-density-of-states.md) per atom per [energy](../../../../energy-split.md), and put $\delta n=n_\uparrow-n_\downarrow$. At fixed total occupation $n$, the two [Hubbard model](../../../../hubbard-model.md) mean-field energies can be written

$$
\varepsilon_{\mathbf k,\uparrow}=\varepsilon_{\mathbf k}+\frac{Un}{2}-\Delta,\qquad \varepsilon_{\mathbf k,\downarrow}=\varepsilon_{\mathbf k}+\frac{Un}{2}+\Delta,\qquad \Delta=\frac{U\delta n}{2}+\mu_0\mu_BH.
$$

The common shift $Un/2$ can be absorbed into the [chemical potential](../../../../chemical-potential-split.md). Lowering the up-spin band by $\Delta$ adds $g_s\Delta$ carriers, while raising the down-spin band removes the same number. Thus

$$
\delta n=2g_s\Delta=Ug_s\delta n+2\mu_0\mu_Bg_sH,\qquad \delta n=\frac{2\mu_0\mu_Bg_s}{1-Ug_s}H.
$$

If $n_a$ is the atom [number density](../../../../number-density.md), the [magnetization](../../../../magnetization.md) is $M=n_a\mu_B\delta n$. The [Stoner-enhanced magnetic susceptibility](../../../../stoner-enhanced-magnetic-susceptibility.md) in SI volume units is therefore

$$
\boxed{\chi=\frac{\partial M}{\partial H}=\frac{2\mu_0n_a\mu_B^2g_s(E_F)}{1-Ug_s(E_F)}=\frac{\chi_P}{1-Ug_s(E_F)}.}
$$

Here $\chi_P$ is the noninteracting [Pauli paramagnetism](../../../../pauli-paramagnetism.md) result. If the paper's $g(E_F)$ counts both spins, $g=2g_s$ and the same result is

$$
\boxed{\chi=\frac{\mu_0n_a\mu_B^2g(E_F)}{1-Ug(E_F)/2}.}
$$

A susceptibility per atom omits $n_a$. Stating the [spin](../../../../spin.md) and volume conventions avoids an otherwise spurious factor of two or a dimensional mismatch.

The [Stoner criterion](../../../../stoner-criterion.md) is $Ug_s(E_F)>1$, equivalently $Ug(E_F)>2$ with spin-summed $g$. To see the instability, transfer $\eta$ [electrons](../../../../electron.md) per atom from one [spin](../../../../spin.md) band to the other. The band-filling cost is $\eta^2/g_s$, whereas the interaction [energy](../../../../energy-split.md) changes by $-U\eta^2$. Their sum $(1/g_s-U)\eta^2$ becomes negative at the threshold. The unpolarized state then ceases to be a local minimum, and nonlinear band filling determines the spontaneous [ferromagnetism](../../../../ferromagnetism.md). The negative continuation of the displayed linear susceptibility beyond the threshold is not a stable paramagnetic response.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
