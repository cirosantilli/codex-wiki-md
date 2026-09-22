<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $m=[E_m]$, $r=V_R[R]$ and $b=V_B[B]$. Saturated [receptor methylation](../../../../receptor-methylation.md) provides a constant positive flux, so the complete balance is

$$
\dot m=r-\frac{bm}{K_B+m}.
$$

At a finite [steady state](../../../../steady-state.md), $r(K_B+m_*)=bm_*$ and therefore

$$
\boxed{m_* =\frac{K_Br}{b-r},\qquad b>r.}
$$

The derivative of the right side is $-bK_B/(K_B+m)^2<0$, so this fixed point is stable in the scalar model. With total [receptor](../../../../receptor-biochemistry.md) [concentration](../../../../concentration.md) $E_T$, it must additionally lie between zero and $E_T$ and leave sufficient [substrate](../../../../substrate-biochemistry.md) for the assumed saturated [receptor methylation](../../../../receptor-methylation.md). If $r\geq b$, the formal equation has no finite positive fixed point: finite [receptor](../../../../receptor-biochemistry.md) capacity then matters.

For an [chemoattractant](../../../../chemoattractant.md) step, activity and hence tumbling frequency fall rapidly before [receptor methylation](../../../../receptor-methylation.md) can change appreciably. Slower chemical modification can then restore [receptor](../../../../receptor-biochemistry.md) signaling and make the tumbling frequency rise toward a new steady value. **[Perfect adaptation](../../../../perfect-adaptation.md)** means return of that output to its original baseline despite the persistent [chemoattractant](../../../../chemoattractant.md) step; it does not mean that [receptor](../../../../receptor-biochemistry.md) [receptor methylation](../../../../receptor-methylation.md) also returns to its original level.

The balance written here alone does not specify how ligand changes activity or [receptor demethylation](../../../../receptor-demethylation.md), and does not yet establish [perfect adaptation](../../../../perfect-adaptation.md). If activity is simply multiplied by a ligand-dependent fraction while this $m$ balance remains unchanged, $m_*$ is unchanged and the activity remains reduced. The following two models add different mechanisms that can compensate for that direct activity reduction.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
