<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the real [eigenfunctions](../../../../../eigenfunction.md), or insert a complex conjugate on the first factor for complex functions. Multiply $-(py_n')'=n^2wy_n$ by $y_m$, do the same with $m,n$ interchanged, and subtract. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
(n^2-m^2)\int_{-1}^1wy_ny_m\,dx=\left[p(y_ny_m'-y_my_n')\right]_{-1}^1=0.
$$

The boundary term vanishes because both functions and derivatives are bounded while $p\to0$. For distinct squared indices, [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md) therefore yields

$$
\boxed{\int_{-1}^1\frac{y_n(x)y_m(x)}{\sqrt{1-x^2}}\,dx=0\qquad(n^2\ne m^2).}
$$

A second integration by parts, using the equation for $y_n$, gives

$$
\int_{-1}^1p\,y_n'y_m'\,dx=[py_n'y_m]_{-1}^1-\int_{-1}^1y_m(py_n')'dx=n^2\int_{-1}^1wy_ny_m\,dx.
$$

Thus [derivative orthogonality when the Sturm-Liouville potential vanishes](../../../../../derivative-orthogonality-when-the-sturm-liouville-potential-vanishes.md) gives

$$
\boxed{\int_{-1}^1y_n'y_m'\sqrt{1-x^2}\,dx=0\qquad(n^2\ne m^2).}
$$

**The index qualification matters.** The source initially allows integer indices, so $n\ne m$ alone does not imply distinct eigenvalues: $m=-n$ gives the same $n^2$. Taking the conventional nonnegative labels $n,m\geq0$ makes the stated conclusion valid. For the polynomial solutions below, $y_{-n}=y_n$, so opposite indices are an explicit counterexample to an unqualified orthogonality claim.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
