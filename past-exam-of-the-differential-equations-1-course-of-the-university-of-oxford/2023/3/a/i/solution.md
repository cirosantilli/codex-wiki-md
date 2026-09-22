<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathcal Pu=u_t-\Delta u+a u_x+b u_y$ on the [unit disk](../../../../../unit-disk.md) over $0<t\leq1$. Smoothness is understood to include continuity on the closed cylinder. If $u$ exceeded its nonnegative [parabolic boundary](../../../../../parabolic-boundary.md) maximum $A$, it would attain a positive global maximum $M>A$ at some spatial interior point at time $t_0>0$. There,

$$
\nabla u=0,\qquad \Delta u\leq0,\qquad u_t\geq0.
$$

At $t_0=1$ the last inequality uses the derivative from the past; at an interior time it is equality. These signs imply $\mathcal Pu+u^3\geq M^3>0$, contradicting the given [differential inequality](../../../../../differential-inequality.md). Thus

$$
\boxed{u\leq A\quad\text{throughout }Q.}
$$

If $A>0$, equality at any point of $Q$ gives the same contradiction with $M=A$, so $u<A$ throughout $Q$. If $A=0$, equality is possible: $u\equiv0$ is an example. More precisely, write the inequality as $\mathcal Pu+c u\leq0$ with $c=u^2\geq0$. The [strong parabolic maximum principle](../../../../../strong-parabolic-maximum-principle.md) shows that an interior zero at time $t_0>0$ forces $u\equiv0$ on $B\times[0,t_0]$.

That conclusion need not extend into the future for a subsolution. For $t_0<1$, take a spatially constant function which is zero for $t\leq t_0$ and equals $-\exp(-1/(t-t_0))$ for $t>t_0$. It is smooth, nonincreasing and nonpositive, so $\mathcal Pu+u^3\leq0$, but it becomes negative after $t_0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
