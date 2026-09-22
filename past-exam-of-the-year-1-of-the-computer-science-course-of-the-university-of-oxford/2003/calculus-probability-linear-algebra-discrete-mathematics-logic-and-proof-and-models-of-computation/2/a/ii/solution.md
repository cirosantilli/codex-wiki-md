<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this [change of variables](../../../../../../change-of-variables-formula.md),

$$
u_x=2x,\quad u_y=-2y,\quad v_x=2y,\quad v_y=2x,
$$

and $u_{xx}+u_{yy}=0=v_{xx}+v_{yy}$. The [second derivative chain rule](../../../../../../second-derivative-chain-rule.md) therefore gives

$$
\begin{aligned}
f_{xx}+f_{yy}
&=g_{uu}(4x^2+4y^2)+2g_{uv}(4xy-4xy)+g_{vv}(4y^2+4x^2)\\
&=4(x^2+y^2)(g_{uu}+g_{vv}).
\end{aligned}
$$

Thus the transformation rule for the [Laplacian](../../../../../../laplacian.md) is

$$
\boxed{\Delta_{x,y}f=4(x^2+y^2)\Delta_{u,v}g.}
$$

For $f=x+y$, its [Laplacian](../../../../../../laplacian.md) is zero. At every point with $(x,y)\ne(0,0)$, division by $4(x^2+y^2)$ proves

$$
\boxed{g_{uu}+g_{vv}=0.}
$$

This conclusion applies to each local inverse branch of the [change of variables](../../../../../../change-of-variables-formula.md): its [Jacobian determinant](../../../../../../jacobian-determinant.md) is $4(x^2+y^2)$, so such a branch exists away from the origin by the [inverse function theorem](../../../../../../inverse-function-theorem.md). A single globally defined $g$ cannot represent $x+y$ on the entire plane, since $(x,y)$ and $(-x,-y)$ give the same $(u,v)$ but generally opposite values of $x+y$. Nor can a differentiable $g$ represent this $f$ in a neighborhood of the origin: the [multivariable chain rule](../../../../../../multivariable-chain-rule.md) there would give $f_x=f_y=0$, contradicting $f_x=f_y=1$. The requested [harmonic function](../../../../../../harmonic-function.md) conclusion is therefore a local statement on nonsingular branches.[Printed p. 2, Question 2(a)(ii)](../../../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-examination-paper-by-the-university-of-oxford-2003.md)

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
