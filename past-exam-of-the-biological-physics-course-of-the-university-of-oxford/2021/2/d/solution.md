<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the simplified [Barkai-Leibler model](../../../../barkai-leibler-model.md), let $M$ be the total methylated [receptor](../../../../receptor-biochemistry.md) [concentration](../../../../concentration.md) and $A=f(S)M$ the active, unoccupied part. Ligand-bound methylated [receptors](../../../../receptor-biochemistry.md) contribute zero activity. Because [CheB](../../../../cheb.md) acts only on active [receptors](../../../../receptor-biochemistry.md),

$$
\dot M=r-\frac{bA}{K_B+A},\qquad r=V_R[R],\quad b=V_B[B].
$$

At a finite [steady state](../../../../steady-state.md),

$$
\boxed{A_* =\frac{K_Br}{b-r},\qquad M_* =\frac{A_*}{f(S)}.}
$$

The output $A_*$ is independent of attractant [concentration](../../../../concentration.md) $S$: attractant changes the necessary [receptor methylation](../../../../receptor-methylation.md) level, while the flux balance fixes activity. This proves [perfect adaptation](../../../../perfect-adaptation.md) for $0<r<b$, $f(S)>0$ and enough methylatable [receptors](../../../../receptor-biochemistry.md). At fixed $S$, $d\dot M/dM=-bf(S)K_B/[K_B+f(S)M]^2<0$, so this [steady state](../../../../steady-state.md) is locally stable. If every [receptor](../../../../receptor-biochemistry.md) is permanently bound, $f=0$, or if the required $M_*$ exceeds the available pool, compensation fails.

This feedback couples demethylation directly to the output. Lower activity lowers demethylation; continuing [CheR](../../../../cher.md) action restores it. The structural dependence on active [receptors](../../../../receptor-biochemistry.md) removes the separate adjustment of $V'_B$ required in [c](../c.md).[Figure 1b and equation 1: saturated modifying flux and output-dependent reverse modification](../../../../robustness-in-simple-biochemical-networks-by-naama-barkai-and-stanislas-leibler.md)

Changing [CheR](../../../../cher.md) or [CheB](../../../../cheb.md) [concentration](../../../../concentration.md) changes $A_*$ and hence the baseline tumbling frequency, but the output still returns to that new baseline after an attractant step within the operating range. Raising [CheR](../../../../cher.md) raises $A_*$; raising [CheB](../../../../cheb.md) lowers it. Adaptation time also changes: linearization gives $\tau=(K_B+A_*)^2/[bf(S)K_B]$. Thus robustness of the return property does not mean an invariant tumbling frequency or response time across different [enzyme](../../../../enzyme-split.md) abundances.

If [CheR](../../../../cher.md) instead has [Michaelis-Menten kinetics](../../../../michaelis-menten-kinetics.md) on the unmethylated pool $U=E_T-M$, its flux is $r(M)=V_R[R](E_T-M)/(K_R+E_T-M)$. Then

$$
\frac{V_R[R](E_T-A/f)}{K_R+E_T-A/f}=\frac{bA}{K_B+A}.
$$

The left side depends on ligand through $f$, even at fixed output $A$; consequently the equilibrium output generally depends on attractant and [perfect adaptation](../../../../perfect-adaptation.md) is lost. It is recovered approximately when $E_T-M\gg K_R$ throughout the response, so the [CheR](../../../../cher.md) flux is effectively saturated.

## ↑ Ancestors (12)

1. [D](../d.md)
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
