<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a twice continuously differentiable function $F$, first check the stationary-point condition $F_x=F_y=0$. Write its [Hessian matrix](../../../../hessian-matrix.md) as $H=\begin{pmatrix}A&B\\B&C\end{pmatrix}$, with $A=F_{xx}$, $B=F_{xy}$ and $C=F_{yy}$. The [second-derivative test](../../../../second-derivative-test.md) uses $D=AC-B^2$: if $D>0$ and $A>0$, the point is a strict local minimum; if $D>0$ and $A<0$, it is a strict local maximum; if $D<0$, it is a saddle point. If $D=0$, the quadratic test is inconclusive and higher-order terms or a direct argument are needed.

For $F=e^{y^2-x^2}$, the first derivatives vanish at the origin and

$$
H(0,0)=\begin{pmatrix}-2&0\\0&2\end{pmatrix},\qquad D=-4<0.
$$

Thus $\boxed{(0,0)\text{ is a saddle point, with }F(0,0)=1}$. Directly, $F(x,0)=e^{-x^2}<1$ for nearby nonzero $x$, while $F(0,y)=e^{y^2}>1$ for nearby nonzero $y$. The presence of both increasing and decreasing directions confirms the [Hessian matrix](../../../../hessian-matrix.md) classification.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [5](../../5.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
