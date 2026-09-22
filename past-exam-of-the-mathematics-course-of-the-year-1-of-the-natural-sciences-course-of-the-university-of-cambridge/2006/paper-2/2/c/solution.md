<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an arbitrary [vector](../../../../../vector.md) $\mathbf x$, expansion in the [orthonormal basis](../../../../../orthonormal-basis.md) gives $x_i=(a_i a_j+b_i b_j+c_i c_j)x_j$, with summation over $j$. Since this holds for every $\mathbf x$, the [resolution of the identity in an orthonormal basis](../../../../../resolution-of-the-identity-in-an-orthonormal-basis.md) is

$$
a_i a_j+b_i b_j+c_i c_j=\delta_{ij}.
$$

Let $P_a=\mathbf a\mathbf a^T$, and similarly for $b,c$. The three [orthogonal projection matrices](../../../../../orthogonal-projection-matrix.md) sum to $I$ and have pairwise products zero. Thus

$$
\boxed{(I-2P_c)(I-2P_b)(I-2P_a)=I-2(P_a+P_b+P_c)=-I,\qquad\mathbf s_{\rm out}=-\mathbf s_{\rm in}.}
$$

Any ray meeting all three ideal perpendicular mirrors therefore returns in the opposite direction, independently of reflection order. This is the geometry of a [corner reflector](../../../../../corner-reflector.md), a kind of [retroreflector](../../../../../retroreflector.md) used in [lunar laser ranging](../../../../../lunar-laser-ranging.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
