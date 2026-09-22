<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The defining relation $yx=x^4y$ lets us move every occurrence of $y$ to the right of every occurrence of $x$. More generally, repeated [conjugation](../../../../conjugation.md) gives

$$
yx^r=x^{4r}y,\qquad y^jx^r=x^{4^jr}y^j.
$$

Negative powers cause no problem because $x^{-1}=x^8$ and $y^{-1}=y^2$. Thus every word in the [group presentation](../../../../group-presentation.md) can be put in the required form, reducing powers using $x^9=y^3=e$:

$$
\boxed{g=x^iy^j,\qquad0\le i\le8,\quad0\le j\le2.}
$$

At this stage existence is proved; uniqueness will follow from the concrete [semidirect product](../../../../semidirect-product.md) in part (b). Moving $x^r$ past $y^j$ gives the multiplication law

$$
\boxed{(x^iy^j)(x^ry^s)=x^{\,i+4^jr\bmod9}y^{\,j+s\bmod3}.}
$$

The action is consistent with reduction of $j$ modulo $3$ because $4^3\equiv1\pmod9$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
