<h1 id="b/5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Test a single discontinuity connecting the two constant initial states. With state 1 below the discontinuity and state 2 above it, their jumps are

$$
[u]=-1,\qquad[uv]=-\sqrt3,\qquad[uv^2+u^2/2]=\tfrac12-(\tfrac32+2)=-3.
$$

The first [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) gives $F'=\sqrt3$, and the second independently gives $(-\sqrt3)F'=-3$, the same value. Since the initial jump is at the origin,

$$
\boxed{F(x)=\sqrt3\,x,\qquad
(u,v)(x,y)=\begin{cases}(2,\sqrt3/2),&y<\sqrt3 x,\\(1,0),&y>\sqrt3 x,\end{cases}\quad x>0.}
$$

Values on the [shock](../../../../../../shock-wave.md) itself do not affect the [weak solution](../../../../../../weak-solution.md). No intermediate state or rarefaction is needed: the prescribed states already lie on the same compressive [shock](../../../../../../shock-wave.md) curve.

For admissibility, the upper-family [characteristic speed](../../../../../../characteristic-speed.md) is $\sqrt3/2+\sqrt2$ behind the [shock](../../../../../../shock-wave.md) and $1$ ahead of it. They satisfy

$$
1<\sqrt3<\sqrt3/2+\sqrt2.
$$

Both lower-family speeds, $-1$ and $\sqrt3/2-\sqrt2$, are less than the [shock](../../../../../../shock-wave.md) speed. These are the [Lax shock admissibility conditions](../../../../../../lax-shock-admissibility-conditions.md) for a family-plus [shock](../../../../../../shock-wave.md). This is the entropy-admissible solution for the [mass](../../../../../../mass.md)/[momentum](../../../../../../momentum-split.md) conservative extension specified by the preceding jump law; imposing an additional velocity [conservation law](../../../../../../conservation-law.md) across the same jump would describe a different problem.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
