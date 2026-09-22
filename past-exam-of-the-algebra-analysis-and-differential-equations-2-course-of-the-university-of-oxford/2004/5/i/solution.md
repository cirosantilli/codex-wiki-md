<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrate $F(z)=e^{iz}/(z^2+1)$ around the real segment from $-R$ to $R$ and the counterclockwise upper semicircle, with $R>1$. The only enclosed [pole](../../../../pole.md) is $i$, whose [residue](../../../../residue.md) is $e^{-1}/(2i)$. On the semicircle, $|e^{iz}|\le1$ and $|z^2+1|\ge R^2-1$, so its integral has magnitude at most $\pi R/(R^2-1)\to0$.

The [residue theorem](../../../../residue-theorem.md) thus gives $\int_{-\infty}^{\infty}e^{ix}/(x^2+1)\,dx=\pi e^{-1}$. The line integral converges absolutely, so taking its real part is justified:

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{x^2+1}\,dx=\frac\pi e.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [5](../../5.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
