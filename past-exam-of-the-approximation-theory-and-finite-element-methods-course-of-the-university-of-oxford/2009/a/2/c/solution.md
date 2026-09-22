<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The monic degree-zero polynomial is $\phi_0=1$. Orthogonality of $x-a$ to one gives $a=\int_0^1x\,dx=1/2$, so $\phi_1=x-1/2$.

The relevant integrals are

$$
\|\phi_0\|_2^2=1,\qquad \|\phi_1\|_2^2=\frac1{12},\qquad
(\phi_1,x\phi_1)=\frac1{24}.
$$

Insert these into the [three-term recurrence for monic orthogonal polynomials](../../../../../three-term-recurrence-for-monic-orthogonal-polynomials.md):

$$
\phi_2=(x-\tfrac12)(x-\tfrac12)-\frac1{12}
=x^2-x+\frac16.
$$

Thus

$$
\boxed{\phi_0=1,\qquad\phi_1=x-\tfrac12,\qquad
\phi_2=x^2-x+\tfrac16.}
$$

Their mutual orthogonality can also be checked directly by integrating on $[0,1]$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
