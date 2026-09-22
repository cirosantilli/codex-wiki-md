<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Detailed balance](../../../../detailed-balance.md) means that at [thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md) each elementary transition and its reverse carry equal [probability](../../../../probability.md) flux. For normalized state [probabilities](../../../../probability.md) $A_{\rm eq}$ and $B_{\rm eq}$,

$$
k_1A_{\rm eq}=k_2B_{\rm eq},\qquad
\frac{B_{\rm eq}}{A_{\rm eq}}=e^{-(G_B-G_A)/(k_BT)}.
$$

With the printed convention $\Delta G_{AB}=G_A-G_B$, the sign is therefore

$$
\boxed{\frac{k_1}{k_2}=e^{\Delta G_{AB}/(k_BT)}}.
$$

The $G$ values are free energies per system, including internal degeneracies; for molar [Gibbs free energies](../../../../gibbs-free-energy.md), replace $k_BT$ by $RT$. If B has lower [free energy](../../../../thermodynamic-free-energy.md), its forward-to-reverse rate ratio exceeds one, as it should.

For constant rates, conservation gives $A=1-B$, so the [master equation](../../../../master-equation.md) is $\dot B=k_1(1-B)-k_2B$. Its [steady state](../../../../steady-state.md) is $B_0=k_1/(k_1+k_2)$, and separation of the decaying deviation yields

$$
B(t)=B_0+[B(0)-B_0]e^{-(k_1+k_2)t},\qquad
\boxed{B(t)=\frac{k_1}{k_1+k_2}(1-e^{-(k_1+k_2)t})}
$$

for the specified initial state A. The relaxation [time constant](../../../../time-constant.md) is $(k_1+k_2)^{-1}$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
