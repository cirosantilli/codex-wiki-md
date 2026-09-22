<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let [chemoattractant](../../../../chemoattractant.md) reduce the activity per methylated [receptor](../../../../receptor-biochemistry.md) by a factor $f$, with $0<f\leq1$, taking the initial factor as one. The active output is $a=fm$. If $V_B$ changes to $V_B'$ but [receptor demethylation](../../../../receptor-demethylation.md) still acts on total methylated [receptor](../../../../receptor-biochemistry.md), the new output is

$$
a_*'=f\frac{K_Br}{V_B'[B]-r}.
$$

Demanding $a_*'=a_* =K_Br/(V_B[B]-r)$ gives

$$
\boxed{V_B'[B]=fV_B[B]+(1-f)r,
\qquad V_B'=fV_B+(1-f)\frac{V_R[R]}{[B]}.}
$$

Reduced [receptor demethylation](../../../../receptor-demethylation.md) lets methylated [receptors](../../../../receptor-biochemistry.md) accumulate to $m_*'=m_*/f$, compensating exactly for their reduced activity. During the transition the activity first falls, then rises as [receptor methylation](../../../../receptor-methylation.md) accumulates. This compensation works only if the required methylated [concentration](../../../../concentration.md) is accessible; in particular $m_*/f<E_T$ in a finite [receptor](../../../../receptor-biochemistry.md) pool.

The required relation contains both [enzyme](../../../../enzyme-split.md) [concentrations](../../../../concentration.md). At fixed rates, increasing [CheR](../../../../cher.md) raises the baseline [receptor methylation](../../../../receptor-methylation.md) and tumbling output, while increasing [CheB](../../../../cheb.md) lowers them. After such a change, the previous fine tuning generally no longer gives [perfect adaptation](../../../../perfect-adaptation.md). For example the required reverse capacity is $b'=fb+(1-f)r$, so changing $r$ without retuning $b'$ changes the adapted output ratio. It is the **precision of adaptation** that is fragile here, in addition to the baseline itself changing. Changing all relevant capacities together in a way preserving the relation is a special exception, not generic robustness.

## ↑ Ancestors (12)

1. [C](../c.md)
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
