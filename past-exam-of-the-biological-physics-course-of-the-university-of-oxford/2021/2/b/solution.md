<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $M=[E_m]$, $r=V_R[R]$ and $b=V_B[B]$. Saturated [CheR](../../../../cher.md) supplies a constant [receptor methylation](../../../../receptor-methylation.md) flux, while [CheB](../../../../cheb.md) removes it with [Michaelis-Menten kinetics](../../../../michaelis-menten-kinetics.md):

$$
\dot M=r-\frac{bM}{K_B+M}.
$$

At a finite [steady state](../../../../steady-state.md), $r(K_B+M_0)=bM_0$, giving

$$
\boxed{M_0=\frac{K_BV_R[R]}{V_B[B]-V_R[R]}=\frac{K_Br}{b-r}.}
$$

It requires $0<r<b$ and $M_0$ below the total available [receptor](../../../../receptor-biochemistry.md) pool. The [steady state](../../../../steady-state.md) is stable because $d\dot M/dM=-bK_B/(K_B+M)^2<0$. If $r\geq b$, the ideal equation has no finite positive [steady state](../../../../steady-state.md); actual methylatable sites would become exhausted.

Attractant binding reduces [receptor](../../../../receptor-biochemistry.md) signalling, reducing [CheA](../../../../chea.md)-dependent [phosphorylation](../../../../phosphorylation.md) of [CheY](../../../../chey.md) and initially reducing tumbling frequency, so smooth runs become longer. A spatially uniform stimulus provides no preferred direction. [Perfect adaptation](../../../../perfect-adaptation.md) means that after this transient the tumbling frequency returns exactly to its pre-step value despite continued attractant presence.

The equation above alone does not specify attractant occupancy or its influence on activity. If binding simply changes activity from $M$ to $fM$ with $0<f<1$, without changing either modifying flux, $M$ remains $M_0$ and the output remains $fM_0$: there is no adaptation. Thus the usual fall followed by recovery requires the additional feedback mechanism developed in [c](../c.md) or [d](../d.md), rather than following from the stated [Michaelis-Menten kinetics](../../../../michaelis-menten-kinetics.md) alone.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
