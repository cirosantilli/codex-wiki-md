<h1 id="5c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the vertex position vectors be $\mathbf a,\mathbf b,\mathbf c,\mathbf d$. Suppose

$$
(\mathbf b-\mathbf a)\cdot(\mathbf d-\mathbf c)=0,
\qquad
(\mathbf c-\mathbf a)\cdot(\mathbf d-\mathbf b)=0.
$$

Subtracting the second scalar product from the first gives

$$
-(\mathbf d-\mathbf a)\cdot(\mathbf c-\mathbf b)=0,
$$

so the remaining pair of [opposite edges of a tetrahedron](../../../../../../opposite-edges-of-a-tetrahedron.md) is also perpendicular.

Put

$$
S_1=|\mathbf b-\mathbf a|^2+|\mathbf d-\mathbf c|^2,
\quad
S_2=|\mathbf c-\mathbf a|^2+|\mathbf d-\mathbf b|^2,
\quad
S_3=|\mathbf d-\mathbf a|^2+|\mathbf c-\mathbf b|^2.
$$

Direct expansion gives, cyclically,

$$
S_1-S_2=-2(\mathbf d-\mathbf a)\cdot(\mathbf c-\mathbf b),
$$

with the other two differences equal to minus twice the scalar products of the other opposite-edge pairs. All three scalar products vanish, hence

$$
\boxed{S_1=S_2=S_3}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5C](../../5c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
