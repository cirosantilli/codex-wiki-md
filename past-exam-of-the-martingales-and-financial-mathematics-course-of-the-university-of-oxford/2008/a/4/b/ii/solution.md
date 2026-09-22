<h1 id="a/4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $f$ is continuous at $x_0$, choose a small interval on which $|f(s)-f(x_0)|<\epsilon/2$. The triangle inequality makes its oscillation less than $\epsilon$, so $\varphi(x_0)=0$.

Conversely, if $\varphi(x_0)=0$, then for every $\epsilon>0$ some $n$ has $\varphi_n(x_0)<\epsilon$. As $x_0$ itself belongs to the interval used in that supremum, $|f(x)-f(x_0)|<\epsilon$ for $|x-x_0|<1/n$. Thus $f$ is continuous at $x_0$.

The [continuity set of a function](../../../../../../continuity-set-of-a-function.md) is therefore

$$
\boxed{\{x:f\text{ is continuous at }x\}
=\bigcap_{m\geq1}\{x:\varphi(x)<1/m\}.}
$$

Each set in the intersection is open by part (i), so this is a [G-delta set](../../../../../../g-delta-set.md) and in particular a Borel set, even if $f$ itself is not measurable.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
