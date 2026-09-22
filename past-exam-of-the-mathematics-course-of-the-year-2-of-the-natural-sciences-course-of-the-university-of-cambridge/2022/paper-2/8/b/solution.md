<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Label the triangle's vertices counterclockwise as $1,2,3$. Let $r$ rotate it by $2\pi/3$ and let $s$ reflect it in the axis through vertex 1 and the midpoint of the opposite side. Then

$$
r^3=e,\qquad s^2=e,\qquad srs=r^{-1}.
$$

The six [dihedral group](../../../../../dihedral-group.md) elements are

$$
\boxed{D_3=\{e,r,r^2,s,rs,r^2s\}.}
$$

The first three are the identity and the rotations by $120^\circ,240^\circ$; the last three are reflections fixing vertices $1,3,2$, respectively. These are all possible symmetries: the image of one vertex has three choices, and the order of the other two has two choices.

Use rightmost-first composition. From the generator relation,

$$
(r^as^b)(r^cs^d)=r^{a+(-1)^bc}s^{b+d},
$$

with exponents reduced modulo three and two. The row-times-column [multiplication table](../../../../../multiplication-table.md) is

$$
\boxed{\begin{array}{c|cccccc}
&e&r&r^2&s&rs&r^2s\\\hline
e&e&r&r^2&s&rs&r^2s\\
r&r&r^2&e&rs&r^2s&s\\
r^2&r^2&e&r&r^2s&s&rs\\
s&s&r^2s&rs&e&r^2&r\\
rs&rs&s&r^2s&r&e&r^2\\
r^2s&r^2s&rs&s&r^2&r&e
\end{array}}
$$

Thus every symmetry is expressed in the two [group generators](../../../../../generator-of-a-group.md) $r,s$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
