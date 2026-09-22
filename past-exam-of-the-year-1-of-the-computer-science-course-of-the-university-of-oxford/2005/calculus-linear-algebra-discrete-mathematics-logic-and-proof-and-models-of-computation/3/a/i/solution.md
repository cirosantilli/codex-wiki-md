<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [homogeneous linear differential equation](../../../../../../homogeneous-linear-differential-equation.md) has solutions $\cos x$ and $\sin x$. Since the forcing is already a homogeneous solution, seek a [particular solution](../../../../../../particular-solution.md) proportional to $x\cos x$. Direct [differentiation](../../../../../../differentiation.md) gives

$$
\left(-\tfrac12x\cos x\right)''-\tfrac12x\cos x=\sin x.
$$

Thus the general solution of the [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation-split.md) is

$$
y=A\cos x+B\sin x-\tfrac12x\cos x.
$$

The first [initial condition](../../../../../../initial-condition.md) gives $A=0$. Also

$$
y'=-A\sin x+B\cos x-\tfrac12\cos x+\tfrac12x\sin x,
$$

so the second [initial condition](../../../../../../initial-condition.md) gives $B-\tfrac12=-\tfrac12$, hence $B=0$. Therefore

$$
\boxed{y(x)=-\tfrac12x\cos x.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2005](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
