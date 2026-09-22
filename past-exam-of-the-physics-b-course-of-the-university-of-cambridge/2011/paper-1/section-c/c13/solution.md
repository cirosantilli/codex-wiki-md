<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

A [microstate](../../../../../microstate.md) specifies the microscopic state: classically the positions and momenta of all particles, or quantum mechanically an allowed many-body state. A [macrostate](../../../../../macrostate.md) specifies a few coarse variables such as [energy](../../../../../energy-split.md), [volume](../../../../../volume.md) and particle number. Many [microstates](../../../../../microstate.md) can give the same [macrostate](../../../../../macrostate.md). A [statistical ensemble](../../../../../statistical-ensemble.md) is a [probability](../../../../../probability.md) assignment over hypothetical copies prepared with the same macroscopic constraints; it does not require a sample to be literally divided into many physical copies. An observable's ensemble mean is $\langle A\rangle=\sum_i p_iA_i$, with an integral replacing the sum in classical [phase space](../../../../../phase-space.md).

For an isolated system at fixed $U,V,N$, the [microcanonical ensemble](../../../../../microcanonical-ensemble.md) assigns equal [probability](../../../../../probability.md) to accessible [microstates](../../../../../microstate.md) in a narrow [energy](../../../../../energy-split.md) shell. If their number is $\Omega(U,V,N)$, the [Boltzmann entropy](../../../../../boltzmann-s-entropy-formula.md) is $S=k_B\ln\Omega$. Thermal contact between two initially isolated systems allows [energy](../../../../../energy-split.md) to be shared while their sum stays fixed. The most probable division maximizes $S_1(U_1)+S_2(U-U_1)$, so equilibrium requires equal $\partial S/\partial U$. This gives the statistical [temperature](../../../../../temperature-split.md) definition

$$
\boxed{\frac1T=\left(\frac{\partial S}{\partial U}\right)_{V,N},\qquad
\beta=\frac1{k_BT}=\left(\frac{\partial\ln\Omega}{\partial U}\right)_{V,N}.}
$$

For positive [temperature](../../../../../temperature-split.md), [energy](../../../../../energy-split.md) tends to [flow](../../../../../flow.md) from lower [entropy](../../../../../entropy-split.md) slope to higher [entropy](../../../../../entropy-split.md) slope until those slopes agree. The narrow energy-shell width represents macroscopic resolution; it must not exclude the physically accessible states.

For a small subsystem exchanging [energy](../../../../../energy-split.md) with a much larger bath, the bath has [energy](../../../../../energy-split.md) $U_{\rm tot}-E_i$ when subsystem [microstate](../../../../../microstate.md) $i$ has [energy](../../../../../energy-split.md) $E_i$. Expanding its [entropy](../../../../../entropy-split.md) gives $S_b(U_{\rm tot}-E_i)=S_b(U_{\rm tot})-E_i/T+\cdots$. Counting compatible bath states therefore yields the [Boltzmann distribution](../../../../../boltzmann-distribution.md) and [canonical ensemble](../../../../../canonical-ensemble-split.md):

$$
p_i=\frac{e^{-\beta E_i}}Z,\qquad Z=\sum_i e^{-\beta E_i},\qquad
U=-\frac{\partial\ln Z}{\partial\beta},\qquad F=-k_BT\ln Z.
$$

The exponential weights individual [microstates](../../../../../microstate.md). An [energy](../../../../../energy-split.md) level of degeneracy $g_j$ has total [probability](../../../../../probability.md) $g_je^{-\beta E_j}/Z$; a more degenerate excited level can outweigh one ground-state level even though each of its [microstates](../../../../../microstate.md) is less probable. The [Gibbs entropy](../../../../../gibbs-entropy.md) $-k_B\sum_i p_i\ln p_i$ gives $S=k_B\ln Z+U/T$. The equilibrium [energy](../../../../../energy-split.md) [variance](../../../../../variance-split.md) is $\langle(\Delta E)^2\rangle=k_BT^2c_V$, linking measurable fluctuations to a macroscopic response.

If particle exchange is also allowed, a reservoir fixes $T$ and [chemical potential](../../../../../chemical-potential-split.md) $\mu$. The [grand canonical ensemble](../../../../../grand-canonical-ensemble.md) weights a state by $e^{-\beta(E_i-\mu N_i)}/\Xi$, with $\Xi=\sum_{N,i}e^{-\beta(E_i-\mu N)}$. Mean particle number is $k_BT\,\partial\ln\Xi/\partial\mu$, while [volume](../../../../../volume.md) remains a constraint in this version. Thus the ensemble follows the physical exchange conditions: fixed [energy](../../../../../energy-split.md), thermal contact, or thermal and particle contact.

In ordinary large short-range systems, relative fluctuations often decrease as $N^{-1/2}$ and the ensembles give the same bulk thermodynamics away from singular limits. Finite systems, critical fluctuations and long-range interactions require care. Interpreting a time average as an [ensemble average](../../../../../expected-value-split.md) additionally requires appropriate sampling or mixing dynamics; it is not guaranteed solely by naming an ensemble. [thermal equilibrium](../../../../../thermal-equilibrium-split.md) [probability](../../../../../probability.md) assignments do not describe every driven or relaxing state.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
