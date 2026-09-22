<h1 id="6c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is the [SIR model with waning immunity](../../../../../../sir-model-with-waning-immunity.md). The [mass-action interaction](../../../../../../mass-action-interaction.md) term $\beta IS$ transfers people from the susceptible compartment to the infected compartment, $\nu I$ transfers infectives to the recovered compartment, and $fR$ returns recovered people to susceptibility as immunity wanes. Adding the equations gives

$$
\frac d{dt}(S+I+R)=0,
$$

so the total population $N$ is conserved.

When $f=0$ and infection is rare, $S\simeq N$ and

$$
I'=(\beta S-\nu)I\simeq(\beta N-\nu)I.
$$

**Thus $I$ initially decays if $\beta N<\nu$. Equivalently, the [basic reproduction number](../../../../../../basic-reproduction-number.md) is $\mathcal R_0=\beta N/\nu<1$, so the [epidemic invasion threshold](../../../../../../epidemic-invasion-threshold.md) is not crossed and no epidemic occurs.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6C](../../6c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
