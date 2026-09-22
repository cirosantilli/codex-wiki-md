<h1 id="a/1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With [constant-effort harvesting](../../../../../../constant-effort-harvesting.md), the constant-effort model is

$$
\boxed{N_{t+1}=g(N_t)-EN_t.}
$$

The extinction multiplier becomes $g'(0)-E$, so extinction is [linearly stable](../../../../../../linear-stability.md) when $g'(0)-1<E<g'(0)+1$. At $E_c=g'(0)-1$ its multiplier crosses $+1$. Values large enough to make the next population negative lie outside the physical validity of this untruncated harvest model.

Any positive [fixed point](../../../../../../fixed-point.md) $N_E$ solves $g(N_E)/N_E=1+E$. Since that ratio is strictly decreasing, there is at most one such point, and it decreases with effort. Differentiating the fixed-point equation yields

$$
\frac{dN_E}{dE}=\frac{N_E}{g'(N_E)-1-E}<0.
$$

If the unharvested positive branch exists, it continues for $0\leq E<E_c$ and approaches zero as $E\uparrow E_c$. This follows because its required ratio lies between $1$ and $g'(0)$; its intersection lies between zero and the unharvested [fixed point](../../../../../../fixed-point.md). There is no positive [fixed point](../../../../../../fixed-point.md) for $E\geq E_c$.

The positive-state multiplier is $m_E=g'(N_E)-E<1$ by [concavity](../../../../../../concave-function.md). It is stable precisely when

$$
\boxed{-1<g'(N_E)-E<1.}
$$

Crossing $-1$ can change stability through a flip, but the direction of change is not fixed by the three assumptions: $dm_E/dE=g''(N_E)N_E'-1$ has no prescribed sign. In the illustrated saturating example, increasing effort eventually removes the positive branch at extinction. The finite upper stability bound for the algebraic extinction map should not be interpreted as a physically meaningful recovery of a population at unrealistically large harvest effort.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
