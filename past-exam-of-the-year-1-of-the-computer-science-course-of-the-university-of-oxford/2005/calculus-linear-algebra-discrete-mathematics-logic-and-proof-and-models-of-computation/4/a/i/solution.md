<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $r>0$, the [chain rule](../../../../../../chain-rule.md) gives $r_x=x/r$ and $r_y=y/r$. Applying it twice to the [radial function](../../../../../../radial-function.md) $u=f(r)$ gives

$$
u_{xx}=f''\frac{x^2}{r^2}+f'\left(\frac1r-\frac{x^2}{r^3}\right),\qquad u_{yy}=f''\frac{y^2}{r^2}+f'\left(\frac1r-\frac{y^2}{r^3}\right).
$$

Using $x^2+y^2=r^2$, [Laplace's equation](../../../../../../laplace-equation.md) becomes

$$
f''+\frac1rf'=0,\qquad (rf')'=0.
$$

Two [integrations](../../../../../../integral-split.md) now give

$$
\boxed{u(x,y)=A\log r+B,\qquad r=\sqrt{x^2+y^2}>0.}
$$

These are the general solutions of the specified [radial function](../../../../../../radial-function.md) form on an [annulus](../../../../../../annulus-mathematics.md) or a punctured plane. If the solution must extend continuously to the origin, the [logarithm](../../../../../../logarithm.md) term forces $A=0$, leaving only a constant [function](../../../../../../function-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
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
