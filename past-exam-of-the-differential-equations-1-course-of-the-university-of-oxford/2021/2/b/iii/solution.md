<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Near $(1,1)$ the [solution of a differential equation](../../../../../solution-of-a-differential-equation.md) has $y>0$, so the [separable differential equation](../../../../../separable-differential-equation.md) gives

$$
\frac{y}{y+1}\,dy=x\,dx,\qquad
y-\log(1+y)=\frac{x^2}{2}+\frac12-\log2.
$$

Equivalently its trajectory lies on the [level set](../../../../../level-set.md)

$$
\boxed{h(x,y):=y-\log(1+y)-\frac{x^2}{2}=\frac12-\log2.}
$$

On $y>0$, the [function](../../../../../function-split.md) $G(y)=y-\log(1+y)$ is [strictly increasing](../../../../../strictly-increasing-function.md) because $G'(y)=y/(1+y)>0$, and its range is $(0,\infty)$. Thus the positive branch exists exactly where

$$
\frac{x^2}{2}+\frac12-\log2>0.
$$

The [connected component](../../../../../connected-component.md) containing $x=1$ is

$$
\boxed{x>x_*:=\sqrt{2\log2-1}\approx0.621526.}
$$

The [implicit function theorem](../../../../../implicit-function-theorem.md) gives a smooth [solution of a differential equation](../../../../../solution-of-a-differential-equation.md) at every such $x$. It remains finite at every finite $x>x_*$, because $G$ increases without bound. As $x\downarrow x_*$, we have $y\downarrow0$, and the original right side $x+x/y$ becomes singular. Hence this is the maximal interval $(x_*,\infty)$ through the prescribed [initial condition](../../../../../initial-condition.md).

In particular, **the solution is not defined for all $x\in(0,2)$**. It cannot pass through $x=x_*$ as a [classical solution](../../../../../classical-solution.md), since its required value there is $y=0$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
