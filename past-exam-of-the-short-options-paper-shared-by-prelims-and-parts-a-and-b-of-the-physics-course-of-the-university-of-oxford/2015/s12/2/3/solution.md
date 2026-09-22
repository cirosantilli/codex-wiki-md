<h1 id="s12/2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Under the simplest interpretation, each spot contains two equally bright, independently bleaching [green fluorescent protein](../../../../../green-fluorescent-protein.md) emitters. Losing one halves the fluorescence and losing the other removes it. A stable [protein dimer](../../../../../protein-dimer.md) carrying one active label per subunit is consistent with this result. The conclusion is two active emitters in the observed spot; it does not by itself rule out unresolved coincident proteins, incomplete fluorescent maturation or blinking. Permanent membrane binding makes loss by dissociation less plausible, but lateral motion out of the observation region would still need experimental control.[stepwise photobleaching as a subunit-counting measurement and its labeling assumptions](../../../../../subunit-counting-in-membrane-bound-proteins-by-maximilian-h-ulbrich-and-ehud-y-isacoff.md)

Let their independent [photobleaching](../../../../../photobleaching.md) times be $T_A,T_B\sim\operatorname{Exp}(k_b)$. Then $t_1=\min(T_A,T_B)$ has rate $2k_b$, while the memoryless remaining lifetime $t_2-t_1$ has rate $k_b$ and mean $1/k_b$, matching the stated single-emitter calibration. The [two-emitter photobleaching completion time](../../../../../two-emitter-photobleaching-completion-time.md) is the maximum, not one single exponential and not a sum of two equal-rate exponential variables. Its [cumulative distribution function](../../../../../cumulative-distribution-function.md) is

$$
P(t_2\leq t)=P(T_A\leq t,T_B\leq t)=(1-e^{-k_bt})^2\qquad(t\geq0).
$$

Differentiating gives its [probability density function](../../../../../probability-density-function.md):

$$
\boxed{f_{t_2}(t)=2k_be^{-k_bt}(1-e^{-k_bt})=2k_b(e^{-k_bt}-e^{-2k_bt}),\quad t\geq0,}
$$

with zero density for $t<0$. It integrates to one, and its mean is $1/(2k_b)+1/k_b=3/(2k_b)$. This uses two active fluorophores at the start of observation, constant illumination and independent irreversible bleaching with the calibrated rate.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2](../../2.md)
3. [S12](../../../s12.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
