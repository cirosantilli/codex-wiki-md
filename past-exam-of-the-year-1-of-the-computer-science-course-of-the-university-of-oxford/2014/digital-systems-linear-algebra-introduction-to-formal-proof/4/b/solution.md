<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Summing the [flow conservation](../../../../../flow-conservation.md) equations over all four junctions cancels every internal flow. The total entering flow is $300+500+250+50+100=1200$, and the known exiting flow is $700+200=900$. Thus

$$
\boxed{f_1=1200-900=300.}
$$

The original arrows point $A\to B$, $C\to A$, $B\to D$, and $C\to D$ for $f_2,f_3,f_4,f_5$, respectively. In particular, $f_1$ exits north from $A$.[Question 4(b) traffic diagram, printed page 5](../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2014.md)

The individual [flow conservation](../../../../../flow-conservation.md) equations are

$$
\begin{aligned}
A:&\quad300+f_3=f_1+f_2,\\
B:&\quad500+250+f_2=f_4,\\
C:&\quad50+100=f_3+f_5,\\
D:&\quad f_4+f_5=700+200.
\end{aligned}
$$

Choose $t=f_5$. Substitution gives all solutions of these [linear equations](../../../../../linear-equation.md):

$$
\boxed{(f_1,f_2,f_3,f_4,f_5)=(300,150-t,150-t,900-t,t),\qquad0\leq t\leq150.}
$$

The inequalities enforce nonnegative flows on all one-way streets. The last junction equation follows from the first three and total [flow conservation](../../../../../flow-conservation.md), so it introduces no further restriction.

The maximum is $\boxed{f_5=150}$. It makes $f_2=f_3=0$. At $A$, all 300 vehicles arriving from the west turn north and leave along $f_1$; none arrives from $C$ or continues east to $B$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
