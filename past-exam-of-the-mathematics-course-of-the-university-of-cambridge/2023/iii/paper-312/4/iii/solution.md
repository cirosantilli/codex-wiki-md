<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In [standard perturbation theory in cosmology](../../../../../../standard-perturbation-theory-in-cosmology.md), $\delta^{(n)}$ is an $n$-leg vertex carrying the symmetrized [standard perturbation theory density kernel](../../../../../../standard-perturbation-theory-density-kernel.md) $F_n$. For [Gaussian random fields](../../../../../../gaussian-random-field.md), a connected four-point diagram with $L$ loops contains $3+L$ linear [power spectra](../../../../../../power-spectrum.md), hence $6+2L$ linear fields.

At tree level the required perturbative-order partitions are

$$
3+1+1+1,
\qquad
2+2+1+1.
$$

The first is a star with one $F_3$ vertex and three linear external legs. The second has two $F_2$ vertices joined by one internal power-spectrum line, with one linear external leg attached to each vertex. At one loop all five partitions of eight into four positive parts are required:

$$
5+1+1+1,
\quad4+2+1+1,
\quad3+3+1+1,
\quad3+2+2+1,
\quad2+2+2+2.
$$

These are conventionally denoted $T_{5111}$, $T_{4211}$, $T_{3311}$, $T_{3221}$, and $T_{2222}$; all inequivalent placements of external legs and all [Wick contractions](../../../../../../wick-contraction.md) are understood. This list is the complete set of [one-loop matter trispectrum](../../../../../../one-loop-matter-trispectrum.md) topologies.

Let $P_a=P_L(k_a)$ and $\mathbf k_{ab}=\mathbf k_a+\mathbf k_b$. With $\sum_a\mathbf k_a=0$, the star contribution is

$$
\boxed{
T_{3111}=6\sum_{d=1}^4
F_3(-\mathbf k_a,-\mathbf k_b,-\mathbf k_c)
P_aP_bP_c},
$$

where $\{a,b,c\}=\{1,2,3,4\}\setminus\{d\}$. For the exchange contribution, sum over the six unordered choices $\{a,b\}$ of linear external legs and let $\{c,d\}$ be the complementary pair:

$$
\boxed{
T_{2211}=4\sum_{\{a,b\}}
P_aP_b\left[
P_L(k_{ac})F_2(-\mathbf k_a,\mathbf k_{ac})
F_2(-\mathbf k_b,-\mathbf k_{ac})
+P_L(k_{ad})F_2(-\mathbf k_a,\mathbf k_{ad})
F_2(-\mathbf k_b,-\mathbf k_{ad})
\right]}.
$$

Thus the connected tree trispectrum is $T_{\rm tree}=T_{3111}+T_{2211}$.

The pressureless single-stream equations cease to be a complete one-loop prediction because loop momenta probe short nonlinear scales and produce ultraviolet-sensitive terms. A consistent result must include the [effective field theory of large-scale structure](../../../../../../effective-field-theory-of-large-scale-structure.md): effective-stress counterterms, including their insertions into the tree topologies, and stochastic terms at the order allowed by [mass conservation](../../../../../../mass-conservation.md) and [momentum conservation](../../../../../../momentum-conservation.md). Their coefficients absorb short-scale dependence and must be fitted or matched. If the observable is a biased tracer rather than matter itself, the corresponding renormalized [bias expansion](../../../../../../bias-expansion.md) is also required.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
