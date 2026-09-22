<h1 id="1/f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The real [cube root](../../../../../../cube-root.md) in the denominator vanishes at $x=-1$, so the printed rule needs the [domain of a function](../../../../../../domain-of-a-function.md) $D_1=\mathbb R\setminus\{-1\}$. On its actual [domain of a function](../../../../../../domain-of-a-function.md), the second [iterated function](../../../../../../iterated-function.md) simplifies to

$$
f(f(x))=
\frac{x/\sqrt[3]{1+x^3}}{\sqrt[3]{1+x^3/(1+x^3)}}
=\frac{x}{\sqrt[3]{1+2x^3}}.
$$

This suggests

$$
\boxed{f^{(n)}(x)=\frac{x}{\sqrt[3]{1+nx^3}},\qquad
D_n=\mathbb R\setminus\{-j^{-1/3}:1\leq j\leq n\}.}
$$

For the induction step, assume the formula at $n$ and restrict to arguments for which its value is not $-1$. Its cube is $x^3/(1+nx^3)$, so another application gives

$$
f(f^{(n)}(x))
=\frac{x/\sqrt[3]{1+nx^3}}{\sqrt[3]{(1+(n+1)x^3)/(1+nx^3)}}
=\frac{x}{\sqrt[3]{1+(n+1)x^3}}.
$$

Real [cube roots](../../../../../../cube-root.md) are multiplicative, including for negative arguments. The newly excluded point satisfies $x^3/(1+nx^3)=-1$, hence $x^3=-1/(n+1)$; all earlier exclusions remain. This proves both the formula and the [domain of a function](../../../../../../domain-of-a-function.md) by [mathematical induction](../../../../../../mathematical-induction.md). The inherited exclusions are essential for an [iteration of a partial function](../../../../../../iteration-of-a-partial-function.md): cancellation in the final expression cannot repair an undefined intermediate application.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [F](../../f.md)
3. [1](../../../1.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
