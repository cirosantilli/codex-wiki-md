<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [finite group](../../../../finite-group.md) action, [Burnside's lemma](../../../../burnside-s-lemma.md) gives

$$
|\Omega/G|=\frac1{|G|}\sum_{g\in G}|\operatorname{Fix}(g)|.
$$

Pair each vertex with its opposite face. This correspondence is equivariant under every tetrahedral symmetry. Each pair has six possible combined color states: three face colors and two vertex colors. Thus we are coloring four positions with six symbols; the two kinds of coloring must be counted together.

The group of rotations is the [alternating group](../../../../alternating-group.md) $A_4$. The identity has four cycles and fixes $6^4$ colorings. Its three half-turns have cycle type $(2,2)$ and each fix $6^2$. Its eight third-turns have cycle type $(3,1)$ and each also fix $6^2$. Consequently the rotation count is

$$
\boxed{\frac{6^4+3\cdot6^2+8\cdot6^2}{12}=141.}
$$

Allowing mirror equivalence gives the full tetrahedral symmetry group $S_4$. Now all permutations of the four paired positions are allowed, so a coloring is determined by a [multiset](../../../../multiset.md) of four symbols chosen from six. [stars and bars](../../../../stars-and-bars-combinatorics.md) gives

$$
\boxed{\binom{6+4-1}{4}=\binom94=126.}
$$

For an independent Burnside check, the five cycle types of $S_4$ give numerator $6^4+6\cdot6^3+3\cdot6^2+8\cdot6^2+6\cdot6=3024$, whose quotient by 24 is 126. This is [paired face and vertex colorings of a tetrahedron](../../../../paired-face-and-vertex-colorings-of-a-tetrahedron.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
