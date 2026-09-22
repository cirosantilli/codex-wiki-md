<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $V=\mathbb R^2$ with basis $e_1,e_2$, the step-two [Lie algebra](../../../../../../lie-algebra-split.md) has basis $e_1,e_2,[e_1,e_2]$ and its last element is central. Write

$$
g(x,y,z)=\exp\bigl(xe_1+ye_2+z[e_1,e_2]\bigr).
$$

Its first level is $v=(x,y)$ and its second level is

$$
\tfrac12v\otimes v+z(e_1\otimes e_2-e_2\otimes e_1).
$$

The step-two multiplication gives

$$
\boxed{(x,y,z)(x',y',z')=
\left(x+x',y+y',z+z'+\tfrac12(xy'-yx')\right).}
$$

Consequently the map

$$
(x,y,z)\longmapsto
\begin{pmatrix}1&x&z+\tfrac12xy\\0&1&y\\0&0&1\end{pmatrix}
$$

is an isomorphism onto the real [Heisenberg group](../../../../../../heisenberg-group.md). The shift by $xy/2$ converts exponential coordinates into the matrix coordinates used for that group. In exponential coordinates the left-invariant horizontal vector fields are

$$
X=\partial_x-\tfrac y2\partial_z,\qquad
Y=\partial_y+\tfrac x2\partial_z,\qquad [X,Y]=\partial_z.
$$

Taking $X,Y$ orthonormal gives exactly the [Carnot-Carathéodory distance](../../../../../../carnot-caratheodory-distance.md) inherited from $G^2(\mathbb R^2)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
