<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the structural [surface charge density](../../../../surface-charge-density.md) stays fixed while a divalent chloride is added, without changing $T$ or $\epsilon$. Let $v=e\phi_0/(k_BT)$ and $\delta c$ be the increment of the bulk divalent [concentration](../../../../concentration.md). Electroneutral addition also increases bulk chloride by $2\delta c$. Varying the squared [Grahame equation](../../../../grahame-equation.md) at fixed $\sigma$ gives

$$
0=\delta c(e^{-2v}+2e^v-3)-\frac e{k_BT}\left[c_{1+}(0)+2c_{2+}(0)-c_{1-}(0)-2c_{2-}(0)\right]\delta\phi_0.
$$

At a strongly negative wall, coions are small. Dropping their contribution to the denominator and $2e^v$ in the numerator gives the requested leading approximation

$$
\boxed{\delta\phi_0\simeq\frac{k_BT}{e}\frac{\delta c(e^{-2v}-3)}{c_{1+}(0)+2c_{2+}(0)}.}
$$

The $-3$ includes the change in bulk osmotic concentration of one added divalent counterion and its two monovalent coions. The numerator's increment is a **bulk** [concentration](../../../../concentration.md); the denominator contains **surface** [concentrations](../../../../concentration.md).[Full differential response before the counterion approximation](../../../../fixed-charge-response-to-added-divalent-chloride.md) Extra counterions screen the wall and make its negative [electric potential](../../../../electric-potential.md) less negative. At fixed bulk [calcium](../../../../calcium.md), $c_{\rm Ca}(0)=c_{\rm Ca}^\infty e^{-2\phi_0/V_T}$ therefore decreases. Under the stipulated proportionality, synaptic activity decreases as well; this argument isolates electrostatic accumulation rather than assuming a separate specific magnesium effect on the [ion channels](../../../../ion-channel.md).

For $\delta c=5\,\mathrm{mM}$, the printed linear approximation gives $\delta\phi_0=9.53434\,\mathrm{mV}$. Linearizing the activity too gives $\delta A/A=-2\delta\phi_0/V_T=-0.7422$, or approximately a $74\%$ reduction. Exponentiating this approximate voltage instead gives $A'/A=0.4761$. **Neither is a controlled finite-increment prediction:** the added divalent [concentration](../../../../concentration.md) is 2.5 times its initial value.

A consistent finite-change calculation is possible within the same [Poisson-Boltzmann equation](../../../../poisson-boltzmann-equation.md). Define, using $\mathrm{mM}$ throughout,

$$
S_m(u)=160(e^u-1)+(2+m)(e^{2u}-1)+(114+2m)(e^{-u}-1)+25(e^{-2u}-1).
$$

Fixed $\sigma$ requires $S_5(u')=S_0(2.84129)$. The physical positive root is $u'=2.58241$, giving

$$
\boxed{\phi'_0=-66.3488\,\mathrm{mV},\quad
\Delta\phi_0=6.65122\,\mathrm{mV},\quad
\frac{A'}A=e^{2(u'-u)}=0.595857.}
$$

Thus the self-consistent finite-change estimate is about a **40.4% reduction**. Both estimates rely on fixed surface charge, ideal ionic activities, and unchanged bulk [calcium](../../../../calcium.md); the limitations of the large local [concentrations](../../../../concentration.md) remain.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
