<h1 id="s12/3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An ATP-binding step with pseudo-first-order rate $k_1c$ has [survival probability](../../../../../survival-probability.md) $S_1=e^{-k_1ct}$ and waiting [density](../../../../../density.md) $P_1=-S_1'=k_1ce^{-k_1ct}$. It decreases from a finite value at zero, integrates to one and has mean $1/(k_1c)$. Its concentration dependence suggests binding-limited waiting before the large 80-degree substep.

Two independent sequential exponential steps of rates $k_a,k_b$ give the convolution

$$
\boxed{P_2(t)=\int_0^t k_ae^{-k_as}k_be^{-k_b(t-s)}ds=\frac{k_ak_b}{k_a-k_b}(e^{-k_bt}-e^{-k_at}).}
$$

It begins at zero, rises to a maximum at $\log(k_a/k_b)/(k_a-k_b)$ and decays; its mean is $k_a^{-1}+k_b^{-1}$. At equal rates it becomes $k^2te^{-kt}$. This supports at least two kinetic events during the waiting associated with the 40-degree substep, plausibly chemical transformation/product release and conformational changes. It does not uniquely identify which rate belongs to hydrolysis or a particular product: different hidden-state networks can have the same waiting distribution. Three 120-degree [catalytic cycles](../../../../../catalytic-cycle.md) per revolution, partitioned into 80 and 40 degrees in the assay, are consistent with three catalytic sites.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [3](../../3.md)
3. [S12](../../../s12.md)
4. [2016](../../../../2016-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
