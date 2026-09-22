<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

If two solutions exist, their difference satisfies $d''+d=0$ with $d(0)=d(L)=0$, where $L=\pi/4$. The general solution is $d=a\sin x+b\cos x$. The first endpoint gives $b=0$ and the second gives $a\sin L=0$, hence $a=0$. Thus the solution is unique if it exists.

For the operator $-D^2-1$, choose the homogeneous solutions $\sin x$ and $\sin(L-x)$ satisfying the left and right endpoint conditions. Continuity at $x=s$ and [derivative](../../../derivative.md) jump $G_x(s^+,s)-G_x(s^-,s)=-1$ yield the [Dirichlet Green function](../../../dirichlet-green-function.md)

$$
\boxed{G(x,s)=\frac{\sin(\min\{x,s\})\sin(L-\max\{x,s\})}{\sin L}.}
$$

Indeed it vanishes at both endpoints and satisfies $-G_{xx}-G=\delta_s$. Splitting the integral at $s=x$ and differentiating verifies that $y=\int_0^LG(x,s)f(s)ds$ is twice continuously differentiable for continuous $f$ and solves the boundary-value problem, establishing existence as well.

At zero, $G_x(0,s)=\sin(L-s)/\sin L=\cos s-\sin s$, since $\cot L=1$. Thus

$$
\boxed{y'(0)=\int_0^{\pi/4}f(s)(\cos s-\sin s)ds.}
$$

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2009](../../2009-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
