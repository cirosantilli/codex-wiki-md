<h1 id="3/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $k=\lfloor y^{1/n}\rfloor$. Because $y>0$, $k$ is a nonnegative [integer](../../../../../../integer-split.md), and

$$
k\leq y^{1/n}<k+1.
$$

The [function](../../../../../../function-split.md) $t\mapsto t^n$ is [strictly increasing](../../../../../../strictly-increasing-function.md) for $t\geq0$, so $k^n\leq y<(k+1)^n$. Both powers are [integers](../../../../../../integer-split.md). Taking the [floor function](../../../../../../floor-function.md) therefore gives

$$
k^n\leq\lfloor y\rfloor<(k+1)^n.
$$

Taking nonnegative $n$th roots now gives $k\leq\lfloor y\rfloor^{1/n}<k+1$. Consequently

$$
\boxed{\left\lfloor\lfloor y\rfloor^{1/n}\right\rfloor=k=\left\lfloor y^{1/n}\right\rfloor.}
$$

The argument also covers $0<y<1$, when both outer [floors](../../../../../../floor-function.md) are zero.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
