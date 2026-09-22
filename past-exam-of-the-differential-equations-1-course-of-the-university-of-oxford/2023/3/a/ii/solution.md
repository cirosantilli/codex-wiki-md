<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With zero drift, choose the [smooth function](../../../../../smooth-function.md)

$$
\boxed{u(x,y,t)=-1+\frac{t}{8}(1-x^2-y^2).}
$$

It equals $-1$ on the entire [parabolic boundary](../../../../../parabolic-boundary.md), so $A=-1$. On the closed cylinder, $-1\leq u\leq-7/8$, while

$$
u_t-\Delta u=\frac{1-x^2-y^2}{8}+\frac t2\leq\frac58.
$$

Consequently

$$
u_t-\Delta u+u^3\leq\frac58-\left(\frac78\right)^3
=-\frac{23}{512}<0.
$$

Nevertheless the maximum at $(0,0,1)$ is

$$
\boxed{\max_{\overline Q}u=-\frac78>-1=A.}
$$

The negative cubic term permits an interior increase while the boundary stays fixed, explaining why the sign condition in the preceding part matters.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
