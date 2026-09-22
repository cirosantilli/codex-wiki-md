<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The **[Picard-Lindelöf theorem](../../../../picard-lindelof-theorem.md)** gives local existence and uniqueness for an [initial value problem](../../../../initial-value-problem.md) when $f$ is continuous on a rectangle around $(a,b)$ and is [Lipschitz continuous](../../../../lipschitz-continuity.md) in its second variable there, with a constant uniform in the first variable. A sufficient hypothesis is that $f$ and $\partial f/\partial y$ are continuous on that rectangle.

More quantitatively, if the rectangle is $|x-a|\leq h_0$, $|y-b|\leq k$, and $|f|\leq M$, a sufficiently small $h>0$ with $h\leq h_0$ and $hM<k$ yields a unique differentiable solution on $[a-h,a+h]$ remaining inside the vertical strip. The proof uses the integral equation

$$
y(x)=b+\int_a^x f(t,y(t))\,dt
$$

and [Picard iteration](../../../../picard-iteration.md), or the [Banach fixed-point theorem](../../../../contraction-mapping-theorem.md) after shrinking $h$ to make the integral operator a contraction. The continuity and Lipschitz hypotheses must hold near the actual initial point.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
