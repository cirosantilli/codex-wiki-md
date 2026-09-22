<h1 id="p/p4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $r=\|u\|_2>0$, and choose $s=1$ if $u_1\geq0$ and $s=-1$ otherwise. Set

$$
w=u+sr e_1.
$$

This vector is nonzero, because $w_1$ has magnitude $|u_1|+r$. Direct computation gives

$$
w^Tu=r(r+su_1),\qquad w^Tw=2r(r+su_1),
$$

so the [Householder transformation](../../../../../householder-transformation.md) satisfies

$$
\boxed{H(w)u=u-2w\frac{w^Tu}{w^Tw}=u-w=-s\|u\|_2 e_1.}
$$

The first entry is nonzero and every other entry is zero. The sign choice also avoids cancellation when forming the first entry of $w$, which is useful in numerical computation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
