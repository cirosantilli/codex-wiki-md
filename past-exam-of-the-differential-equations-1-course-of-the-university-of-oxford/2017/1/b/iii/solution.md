<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $k>2$ and choose the positive [Dulac function](../../../../../dulac-function.md)

$$
\psi(x,y)=\exp\!\left(-\frac{2(x+y)}{k-2}\right).
$$

More generally, for $\psi=e^{a(x+y)}$, direct differentiation gives

$$
\nabla\cdot(\psi(X,Y))=\psi\bigl[3+(-2+(2-k)a)x-ax^2\bigr].
$$

Taking $a=-2/(k-2)$ cancels the linear term and makes the quadratic term nonnegative:

$$
\boxed{\nabla\cdot(\psi(X,Y))=\psi\left(3+\frac{2x^2}{k-2}\right)>0.}
$$

The open positive quadrant is [simply connected](../../../../../simply-connected-space.md), so the [Bendixson-Dulac theorem](../../../../../bendixson-dulac-theorem.md) excludes every nonconstant [periodic orbit](../../../../../periodic-orbit.md) entirely inside it. Such an orbit cannot touch $x=0,y>0$ while staying in the closed quadrant, since its differentiable coordinate $x$ would have a local minimum there but $\dot x=-y\ne0$. The same argument applies on $y=0,x>0$. It cannot pass through the origin either, by local uniqueness of this smooth [autonomous system](../../../../../autonomous-system-mathematics.md). Therefore **there is no nonconstant closed trajectory in the entire nonnegative quadrant**. The calculation illustrates an [exponential Dulac multiplier for a quadratic planar system](../../../../../exponential-dulac-multiplier-for-a-quadratic-planar-system.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
