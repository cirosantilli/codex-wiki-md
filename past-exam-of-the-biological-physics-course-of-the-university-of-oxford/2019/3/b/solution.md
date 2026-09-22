<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $h=K/S$, require $0<h<1$, and use the dimensionless time $s=\alpha t$. While X is produced, $X/S=1-e^{-s}$; afterwards $X/S=(1-e^{-\alpha T})e^{-\alpha(t-T)}$. X crosses the activation threshold on its rising branch at

$$
t_a=\frac{-\ln(1-h)}\alpha.
$$

Symmetry keeps $Y=Z$. They initially receive production through X alone and need another interval $t_a$ of active input to reach $K$. If this happens while X is still above threshold, their mutual OR activation sustains production permanently. X remains above $K$ until

$$
t_b=T+\frac1\alpha\ln\frac{1-e^{-\alpha T}}h
=\frac1\alpha\ln\frac{e^{\alpha T}-1}h.
$$

The [persistence correction to a gene-circuit pulse threshold](../../../../persistence-correction-to-a-gene-circuit-pulse-threshold.md) uses the limiting latch condition is $t_b=2t_a$, yielding

$$
\boxed{T_{\min}=\frac1\alpha\ln\left(1+\frac{h}{(1-h)^2}\right).}
$$

For $T>T_{\min}$, $Y$ and $Z$ cross their common threshold and approach $S$ even after X decays away. For $T<T_{\min}$ they either remain zero or make a subthreshold pulse and return to zero. Exact equality is sensitive to the convention for the ideal threshold, so robust switching requires a strict excess. At $h=1/2$, $T_{\min}=\ln3/\alpha$, whereas $Y$ and $Z$ cross at $2\ln2/\alpha$ in absolute time.

The shorter required _production duration_ reflects X's persistence after production stops. Requiring $T\ge2t_a$ would incorrectly discard that tail when all activating [ligands](../../../../ligand-biochemistry.md) remain present. If $K\ge S$, no finite pulse reaches the required feedback-active state. The second panel of the figure in [solution](../a/solution.md) contrasts pulses shorter and longer than $\ln3/\alpha$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
