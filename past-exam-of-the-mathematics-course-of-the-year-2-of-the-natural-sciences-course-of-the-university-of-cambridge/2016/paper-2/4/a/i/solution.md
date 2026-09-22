<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $0<\arg z<2\pi$, so $\sqrt z=\sqrt R\,e^{i\theta/2}$ on the arc. Its clockwise orientation gives

$$
I(R)=i\sqrt R\int_{3\pi/2}^{\pi/2}f(Re^{i\theta})e^{i\theta/2}\,d\theta.
$$

Because $f$ is an [analytic function](../../../../../../holomorphic-function-split.md) at zero, $f(Re^{i\theta})=f(0)+O(R)$ uniformly on the small arc. Integration then gives

$$
I(R)=2\sqrt R f(0)\big(e^{i\pi/4}-e^{3i\pi/4}\big)+O(R^{3/2})=2\sqrt{2R}\,f(0)+O(R^{3/2}).
$$

Therefore

$$
\boxed{\lim_{R\to0}I(R)=0.}
$$

The [estimation lemma](../../../../../../estimation-lemma.md) also gives $|I(R)|\leq\pi\sqrt R\max_C|f|$. Hence a sufficient large-arc condition is

$$
\boxed{\max_C|f(z)|=o(R^{-1/2})\quad(R\to\infty).}
$$

For example $f(z)=O(|z|^{-1/2-\eta})$ uniformly on the arc, with $\eta>0$, suffices. Under the stronger literal assumption that $f$ is analytic at infinity, its Laurent expansion is $f(z)=f(\infty)+O(1/z)$; the necessary and sufficient condition is then $f(\infty)=0$. A nonzero constant term would instead give the growing contribution $2\sqrt{2R}f(\infty)$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
