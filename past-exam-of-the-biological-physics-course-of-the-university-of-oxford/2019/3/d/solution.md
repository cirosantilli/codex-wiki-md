<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $x=X/S$, $y=Y/S$, $z=Z/S$, $h=K/S$ and $s=\alpha t$. The [repressilator](../../../../repressilator.md) in the stated [logic approximation](../../../../logic-approximation-for-gene-regulation.md) is

$$
\boxed{\frac{dx}{ds}=H(h-z)-x,\quad
\frac{dy}{ds}=H(h-x)-y,\quad
\frac{dz}{ds}=H(h-y)-z,\quad(x,y,z)(0)=(0,1,0).}
$$

Assume $0<h<1$. Initially low Z allows X production; high Y blocks Z; and Y is initially at its unrepressed steady level. X first rises through $h$ at $s_1=a=-\ln(1-h)$, turning Y production off. Y then decays through $h$ at $s_2=a+b$, where $b=-\ln h$, allowing Z to rise. Z reaches $h$ at $s_3=2a+b$ and switches X production off. At this point $x_3=1-h(1-h)^2$, so X falls through $h$ at $s_4=s_3+\ln(x_3/h)$ and releases Y production.

Y's rise then switches Z off, Z's fall releases X again, and the sequence repeats. Every segment is exponential relaxation towards one if its production gate is on, or towards zero if off. For a rising segment starting at $v_0<h$, the next threshold time is $\ln[(1-v_0)/(1-h)]$; for a falling segment starting at $v_0>h$, it is $\ln(v_0/h)$. These rules determine the whole trace without pretending the [concentrations](../../../../concentration.md) are square waves. X, Z and Y peak in sequence after the stated initial condition; the last panel of the figure in [solution](../a/solution.md) gives an illustrative $h=1/2$ trajectory.

The delayed sequence of three inhibitory links supplies [negative feedback](../../../../negative-feedback.md) with finite response times. Equal rates make the cycling symmetric after the initial transient, not simultaneous. If $h\ge1$, repression is never reliably engaged and the [proteins](../../../../protein-split.md) approach their unrepressed levels instead; oscillation is not implied for arbitrary thresholds or for every smooth regulatory law replacing the ideal relay.

## ↑ Ancestors (12)

1. [D](../d.md)
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
