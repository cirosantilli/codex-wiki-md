<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Define the [linear map](../../../../../linear-map.md) $A:\mathbb R^5\to\mathbb R^2$ by the two prescribed left-hand sides. Then $V=\ker A$, so it is a [vector subspace](../../../../../vector-subspace.md): it contains zero, and linear combinations of vectors with zero image still have zero image.

Subtract the first equation from the second to obtain $a_2=-2a_3-3a_4-4a_5$. The first equation then gives $a_1=a_3+2a_4+3a_5$. Consequently

$$
(a_1,a_2,a_3,a_4,a_5)=a_3(1,-2,1,0,0)+a_4(2,-3,0,1,0)+a_5(3,-4,0,0,1).
$$

Each of the three displayed vectors satisfies both equations, and the decomposition proves they span $V$. If their linear combination is zero, its third, fourth and fifth coordinates respectively force all three coefficients to vanish. They are therefore [linearly independent](../../../../../linear-independence.md), giving the [basis](../../../../../basis.md)

$$
\boxed{\{(1,-2,1,0,0),\ (2,-3,0,1,0),\ (3,-4,0,0,1)\},\qquad\dim V=3.}
$$

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
