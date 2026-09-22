<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [wave equation](../../../../../../wave-equation-split.md) with wave speed one, [D'Alembert's formula](../../../../../../d-alembert-s-formula.md) with arbitrary twice continuously differentiable initial displacement $h(x)=u(x,0)$ is

$$
u(x,t)=\frac{h(x+t)+h(x-t)}2+\frac12\int_{x-t}^{x+t}g(s)\,ds.
$$

The arbitrary [function](../../../../../../function-split.md) $h$ is essential: only the initial velocity is prescribed. For $g=0$, this gives

$$
\boxed{u(x,t)=\frac{h(x+t)+h(x-t)}2.}
$$

Both travelling terms solve the [wave equation](../../../../../../wave-equation-split.md), and their [time derivatives](../../../../../../time-derivative.md) cancel at $t=0$. Conversely every classical solution has this form for its initial displacement $h$.

## ↑ Ancestors (13)

1. [I](../i.md)
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
