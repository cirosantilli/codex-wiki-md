<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the product identity $\sin z\cos z=\tfrac12\sin2z$ to decompose the initial shape:

$$
y(x,0)=A\sin\frac{\pi x}l+\frac A2\sin\frac{2\pi x}l.
$$

The [Fourier sine series](../../../../fourier-sine-series.md) is already explicit. Zero initial velocity gives cosine time factors, so

$$
\boxed{A_1=A,\qquad A_2=A/2,\qquad A_n=0\ (n\geq3),}
$$

and $y(x,t)=A\sin(\pi x/l)\cos(\pi ct/l)+(A/2)\sin(2\pi x/l)\cos(2\pi ct/l)$. Orthogonality of the sine modes makes this decomposition unique in the usual square-integrable fixed-end setting.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [11](../../11.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
