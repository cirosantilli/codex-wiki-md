<h1 id="section-b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Pauli matrix](../../../../../pauli-matrices.md) $\sigma_x$ flips the [spin](../../../../../spin.md) with unit [matrix element](../../../../../matrix-element.md). A nonzero oscillator [matrix element](../../../../../matrix-element.md) changes exactly one [occupation number](../../../../../occupation-number.md), through a [creation operator](../../../../../creation-operator.md) or an [annihilation operator](../../../../../annihilation-operator.md):

$$
\langle n_j+1|a_j^\dagger|n_j\rangle=\sqrt{n_j+1},\qquad
\langle n_j-1|a_j|n_j\rangle=\sqrt{n_j}.
$$

For a [spin](../../../../../spin.md) flip, the spin energy change divided by $\hbar$ is $-s_\sigma\Omega$. Thus creation and annihilation in mode $j$ have total frequency changes $\omega_j-s_\sigma\Omega$ and $-\omega_j-s_\sigma\Omega$, respectively. Distinct modes or different occupation changes lead to orthogonal final [quantum states](../../../../../quantum-state.md), so their [probabilities](../../../../../probability.md) add. [Fermi's golden rule](../../../../../fermi-s-golden-rule.md) consequently gives

$$
|c_{\eta\sigma}(t)|^2=\frac{2\pi\lambda^2t}{\hbar^2}
\sum_j\left[(n_j+1)\delta(\omega_j-s_\sigma\Omega)
+n_j\delta(\omega_j+s_\sigma\Omega)\right],\quad \eta\ne\sigma.
$$

The [Dirac delta function](../../../../../dirac-delta-function.md) is even, accounting for the sign in the annihilation term. Since all $\omega_j,\Omega>0$, an initially up spin can only emit an oscillator quantum, while an initially down spin can only absorb one. Writing the oscillator [density of states](../../../../../density-of-states.md) per unit angular frequency as $g(\omega)=\sum_j\delta(\omega-\omega_j)$, the continuum limit gives

$$
\boxed{|c_{\eta\sigma}(t)|^2=\frac{2\pi\lambda^2t}{\hbar^2}
\begin{cases}g(\Omega)(n_\Omega+1),&\sigma=\uparrow,\\
g(\Omega)n_\Omega,&\sigma=\downarrow,
\end{cases}\quad\eta\ne\sigma.}
$$

The $+1$ permits emission even from the oscillator vacuum; absorption requires a quantum already present. The notation $n_\Omega$ assumes a common or smoothly specified occupation at the resonant frequency. If several resonant modes have different occupations, it denotes their [density of states](../../../../../density-of-states.md) weighted mean, so that $g(\Omega)n_\Omega=\sum_j n_j\delta(\Omega-\omega_j)$ after continuum smoothing. This is the [golden-rule relaxation of a spin coupled to an oscillator bath](../../../../../golden-rule-relaxation-of-a-spin-coupled-to-an-oscillator-bath.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
