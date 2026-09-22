<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $t=\tan u$ with the inverse tangent branch $-\pi/2<u<\pi/2$. Then $dt/(1+t^2)=du$, so

$$
\boxed{\int_0^x\frac{dt}{1+t^2}=\arctan x.}
$$

For $|t|<1$, the [geometric series](../../../../geometric-series.md) gives $(1+t^2)^{-1}=1-t^2+t^4-t^6+\cdots$. Integrating term by term on compact subintervals of $(-1,1)$ produces

$$
\boxed{\arctan x=x-\frac{x^3}{3}+\frac{x^5}{5}-\frac{x^7}{7}+O(x^9).}
$$

The integral identity itself holds for every real $x$; the displayed local power-series argument uses $|x|<1$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
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
