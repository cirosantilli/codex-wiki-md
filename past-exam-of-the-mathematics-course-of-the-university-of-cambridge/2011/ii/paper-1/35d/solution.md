<h1 id="35d/solution">Solution</h1>

↑ **Parent:** [35D](../35d.md)

The [microcanonical ensemble](../../../../../microcanonical-ensemble.md) describes an isolated system at fixed energy, volume and particle number. The [canonical ensemble](../../../../../canonical-ensemble.md) describes fixed particle number and volume with heat exchange at a prescribed temperature. The [grand canonical ensemble](../../../../../grand-canonical-ensemble.md) additionally allows particles to exchange with a reservoir, prescribing temperature, volume and chemical potential. Their respective equilibrium probabilities are uniform on the accessible energy shell, proportional to $e^{-\beta E_n}$, and proportional to $e^{-\beta(E_n-\mu N_n)}$. For stable short-range systems in the [thermodynamic limit](../../../../../thermodynamic-limit.md), concentration of relative energy and particle-number fluctuations and concavity of entropy make their bulk predictions equivalent; phase coexistence or nonadditive interactions require care.

For the microcanonical case restrict the allowed states to the fixed-energy shell of size $\Omega$, imposing $p_n=0$ outside it. Maximize the [Gibbs entropy](../../../../../gibbs-entropy.md) subject to $\sum p_n=1$. A [Lagrange multiplier](../../../../../lagrange-multiplier.md) gives $-k_B(\log p_n+1)+\lambda=0$ on the shell, so

$$
\boxed{p_n=1/\Omega\text{ on the shell},\qquad S=k_B\log\Omega.}
$$

For the canonical case impose both normalization and $\sum p_nE_n=U$. Stationarity of $-k_B\sum p_n\log p_n-\lambda(\sum p_n-1)-k_B\beta(\sum p_nE_n-U)$ gives $p_n\propto e^{-\beta E_n}$. Thus

$$
\boxed{p_n=e^{-\beta E_n}/Z,\qquad Z=\sum_ne^{-\beta E_n},\qquad\beta=(k_BT)^{-1}.}
$$

The last identification follows from $\partial S/\partial U=1/T$. Entropy is strictly concave in the probabilities, so these stationary distributions are maxima.

For the independent three-level particles, put $z=\epsilon/(k_BT)$ and $Z_1=1+2\cosh z$. The full [partition function](../../../../../canonical-partition-function.md) is $Z_1^N$ because the particles occupy labeled lattice sites. Differentiation gives

$$
\boxed{\overline E=-\frac{2N\epsilon\sinh z}{1+2\cosh z},\qquad C=Nk_Bz^2\frac{2\cosh z+4}{(1+2\cosh z)^2}.}
$$

The heat capacity also equals $N\operatorname{Var}(E_1)/(k_BT^2)$, confirming positivity. As $T\to+\infty$, the three occupations become equal:

$$
\boxed{\overline E\sim-\frac{2N\epsilon^2}{3k_BT}\to0,\qquad C\sim\frac{2N\epsilon^2}{3k_BT^2}\to0.}
$$

As $T\downarrow0$, all particles occupy their unique lowest state:

$$
\boxed{\overline E=-N\epsilon+N\epsilon e^{-z}+O(e^{-2z}),\qquad C\sim Nk_Bz^2e^{-z}\to0.}
$$

A [negative temperature](../../../../../negative-temperature.md) is possible because the total energy is bounded above. An equilibrated population inversion has more particles at $+\epsilon$ than at $-\epsilon$. For example probabilities $(p_-,p_0,p_+)=(1,2,4)/7$ correspond to $T=-\epsilon/(k_B\log2)$ and mean energy $3N\epsilon/7$. This is a macroscopic occupation pattern; an isolated individual microstate is not itself assigned a temperature. At the positive zero-temperature limit the ground state is unique, so the entropy tends to zero: **the system obeys the third law of thermodynamics**. The negative-temperature branch likewise approaches the unique highest-energy state as $T\to0^-$; it does not introduce residual ground-state entropy.

## ↑ Ancestors (11)

1. [35D](../35d.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
