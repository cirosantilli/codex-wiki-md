<h1 id="analysis/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the branch in (i) and the positively oriented slit-annulus contour. Its upper ray runs from $r$ to $R$, its outer circle counterclockwise, its lower ray from $R$ back to $r$, and its inner circle clockwise. Initially keep their arguments at $\alpha$ and $2\pi-\alpha$ as in the figure, with $0<\alpha<\pi/2$; let $\alpha\downarrow0$ for fixed $0<r<1<R$. Both poles $i,-i$ lie inside.

Write $\sigma=\Re w\in(-1,1)$. On the outer circle the absolute integral is $O(R^{\sigma-1})$, since $|z^w|\le e^{2\pi|\Im w|}R^\sigma$ and $|z^2+1|\ge R^2-1$. On the inner circle it is $O(r^{\sigma+1})$. Both tend to zero. The real integral converges absolutely because its endpoint behaviors are $x^\sigma$ and $x^{\sigma-2}$.

The two residues, with the chosen arguments, are

$$
\frac{e^{i\pi w/2}}{2i},\qquad-\frac{e^{3i\pi w/2}}{2i}.
$$

The [residue theorem](../../../../../residue-theorem.md) and the two ray orientations therefore give

$$
(1-e^{2\pi iw})I(w)=\pi e^{i\pi w/2}(1-e^{i\pi w}),\qquad I(w)=\int_0^\infty\frac{x^w}{1+x^2}\,dx.
$$

For $w\ne0$ in this strip we may cancel $1-e^{i\pi w}$; its only possible zero here is $w=0$. Consequently

$$
\boxed{I(w)=\frac{\pi e^{i\pi w/2}}{1+e^{i\pi w}}=\frac\pi{2\cos(\pi w/2)}.}
$$

At $w=0$ the same result follows directly from $I(0)=\int_0^\infty(1+x^2)^{-1}dx=\pi/2$, or by [dominated convergence](../../../../../dominated-convergence-theorem.md). The denominator has no zero in the open strip.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Analysis](../../../analysis.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
