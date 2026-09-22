<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Apply the [residue theorem](../../../residue-theorem.md) to $F(z)=(z^2+4)^{-2}$ on the upper semicircle of radius $R>2$, traversed counterclockwise. Its sole enclosed [pole](../../../pole.md) is the double pole at $2i$, and

$$
\operatorname{Res}_{z=2i}F
=\left.\frac d{dz}(z+2i)^{-2}\right|_{z=2i}
=-\frac2{(4i)^3}=-\frac i{32}.
$$

On the semicircular arc, $|z^2+4|\ge R^2-4$, so the [ML inequality](../../../estimation-lemma.md) bounds its contribution by $\pi R/(R^2-4)^2\to0$. The real integral is absolutely convergent, since its integrand is $O(|x|^{-4})$ at infinity. Taking $R\to\infty$ in the contour identity yields

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{(x^2+4)^2}=2\pi i\left(-\frac i{32}\right)=\frac\pi{16}.}
$$

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2006](../../2006-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
