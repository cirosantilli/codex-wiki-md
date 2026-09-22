<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To include all momentum-dependent contributions to the [two-point function](../../../../../two-point-correlation-function.md), put one external line at each [interaction vertex](../../../../../interaction-vertex.md). Let $r$ be the number of lines connecting the vertices, and $t_A,t_B$ their numbers of [tadpole diagrams](../../../../../tadpole-diagram.md). For vertex valences $v_A,v_B\in\{4,6\}$,

$$
r+2t_A=v_A-1,\qquad r+2t_B=v_B-1.
$$

The integer $r$ is odd, and $r=1$ gives a [one-particle-reducible Feynman diagram](../../../../../one-particle-reducible-feynman-diagram.md) and is excluded. Thus the complete list is

- $v_A=v_B=4$: $r=3$, $t_A=t_B=0$, the [sunset diagram](../../../../../sunset-diagram.md).
- $v_A=4,v_B=6$: $r=3$, $t_A=0,t_B=1$, the [sunset diagram](../../../../../sunset-diagram.md) with one [tadpole diagram](../../../../../tadpole-diagram.md).
- $v_A=v_B=6$: $r=3$, $t_A=t_B=1$, the [sunset diagram](../../../../../sunset-diagram.md) with one [tadpole diagram](../../../../../tadpole-diagram.md) at each vertex.
- $v_A=v_B=6$: $r=5$, $t_A=t_B=0$, the [five-line banana integral](../../../../../five-line-banana-integral.md) topology.

The coefficient of the mixed graph includes the reflected external attachment as well as its reciprocal [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md). If both external lines attach to the same [interaction vertex](../../../../../interaction-vertex.md), no external [momentum](../../../../../momentum-split.md) enters the connecting internal lines, and that [Feynman diagram](../../../../../feynman-diagram.md) cannot contribute to [wave-function renormalization](../../../../../wave-function-renormalization.md).

For incoming external [momentum](../../../../../momentum-split.md) $p$, assign the connecting lines [momenta](../../../../../momentum-split.md) $k_1,\ldots,k_{r-1},p-\sum_jk_j$. Define

$$
B_{r,M}(p)=\int\prod_{j=1}^{r-1}\frac{d^3k_j}{(2\pi)^3}
\left[\prod_{j=1}^{r-1}D(k_j)\right]D\!\left(p-\sum_{j=1}^{r-1}k_j\right),\qquad r=3,5.
$$

The [momentum space](../../../../../momentum-space.md) [Feynman rules](../../../../../feynman-rules.md) give, in the order listed,

$$
\boxed{\begin{aligned}
&C_{44}(-ig_1)^2B_{3,M}(p),\\
&C_{46}(-ig_1)(-ig_2)T_MB_{3,M}(p),\\
&C_{66,3}(-ig_2)^2T_M^2B_{3,M}(p),\\
&C_{66,5}(-ig_2)^2B_{5,M}(p).
\end{aligned}}
$$

Each $C$ is a reciprocal [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md), including any equivalent external attachments. There are respectively $2,3,4,4$ independent [loop momenta](../../../../../loop-momentum.md).

**If “contribute to wavefunction renormalization” means requiring a divergent kinetic counterterm after subtraction of all subdivergences, only the last topology qualifies.** The first three still have nontrivial external [momentum](../../../../../momentum-split.md) dependence and give finite contributions to a normalization condition; their raw divergent factors arise from [mass counterterms](../../../../../mass-counterterm.md) and [interaction vertex](../../../../../interaction-vertex.md) [counterterms](../../../../../counterterm.md). Keeping all four here makes this distinction explicit. The [ultraviolet divergence](../../../../../ultraviolet-divergence.md) analysis in [d](../../d.md) establishes it directly.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum field theory course of the University of Oxford](../../../../split.md)
6. [Quantum field theory course of the University of Oxford](../../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
