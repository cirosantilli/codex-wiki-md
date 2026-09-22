<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here the velocity contribution in [D'Alembert's formula](../../../../../../d-alembert-s-formula.md) is

$$
\frac12\int_{x-t}^{x+t}e^s\,ds=\frac{e^{x+t}-e^{x-t}}2=e^x\sinh t.
$$

Thus, with arbitrary twice continuously differentiable $h$,

$$
\boxed{u(x,t)=\frac{h(x+t)+h(x-t)}2+e^x\sinh t.}
$$

For the added term, $u_{tt}=e^x\sinh t=u_{xx}$ and $u_t(x,0)=e^x\cosh0=e^x$. Its displacement at $t=0$ is zero, leaving $h$ free as required.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
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
