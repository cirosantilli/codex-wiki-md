<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $a=\pi/2$. Substituting $x=-a$ and $x=a$ into part (ii), using $\cos(\pi/4)=\sin(\pi/4)=1/\sqrt2$, gives

$$
-1+\frac{e^a}{\sqrt2}(A-B)=e^a,
\qquad
1+\frac{e^{-a}}{\sqrt2}(A+B)=e^{-a}.
$$

Thus $A-B=\sqrt2(1+e^{-a})$ and $A+B=\sqrt2(1-e^a)$. Solving these two [linear equations](../../../../../../linear-equation.md) gives

$$
A=\sqrt2(1-\sinh a),\qquad B=-\sqrt2\cosh a.
$$

Consequently the solution of the [boundary value problem](../../../../../../boundary-value-problem-split.md) is

$$
\boxed{y(x)=\sin x+\sqrt2 e^{-x}\left[\left(1-\sinh\frac\pi2\right)\cos\frac x2-\cosh\frac\pi2\sin\frac x2\right].}
$$

The two independent [boundary conditions](../../../../../../boundary-condition.md) determine $A,B$ uniquely.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
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
