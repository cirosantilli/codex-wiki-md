<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u$ be the [allele frequency](../../../../../../allele-frequency.md) of $A$, with [random mating](../../../../../../panmixia.md) and sufficiently large population size to neglect [genetic drift](../../../../../../genetic-drift.md). The [Hardy-Weinberg proportions](../../../../../../hardy-weinberg-principle.md) before selection are $u^2,2u(1-u),(1-u)^2$. Write the three [genotype fitnesses](../../../../../../genotype-fitness.md) as $w_{AA},w_{Aa},w_{aa}$, with $w_{Aa}$ smaller than either [homozygote](../../../../../../homozygote.md) value. After one viability-selection generation,

$$
u'=\frac{w_{AA}u^2+w_{Aa}u(1-u)}{\bar w},
\qquad \bar w=w_{AA}u^2+2w_{Aa}u(1-u)+w_{aa}(1-u)^2.
$$

Consequently

$$
u'-u=\frac{u(1-u)}{\bar w}
\left[(w_{AA}-w_{Aa})u-(w_{aa}-w_{Aa})(1-u)\right].
$$

Put $a=w_{AA}-w_{Aa}>0$, $b=w_{aa}-w_{Aa}>0$. The [underdominant allele-frequency dynamics](../../../../../../underdominant-allele-frequency-dynamics.md) has stable fixation states zero and one, separated by the unstable threshold

$$
\boxed{u_c=\frac b{a+b}.}
$$

Below it $A$ decreases to [allele fixation](../../../../../../allele-fixation.md) of $a$; above it $A$ increases to fixation. Exactly at the threshold the deterministic frequency remains balanced, but any perturbation selects a side. This is [underdominance](../../../../../../underdominance.md), or [heterozygote disadvantage](../../../../../../underdominance.md), rather than balancing selection from [heterozygote advantage](../../../../../../heterozygote-advantage.md).

In a continuous-time weak-selection or selection-rate convention, the corresponding equation is $\dot u=u(1-u)[(a+b)u-b]$. Equal [homozygote](../../../../../../homozygote.md) fitness gives $\dot u=su(1-u)(2u-1)$ for a positive selection strength $s$. The next part uses this explicitly stated continuous-time convention; $s$ and migration then have the same time units.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
