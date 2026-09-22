<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Label the physical qubits by $(i,j)$, with outer block $1\leq i\leq n$ and inner position $1\leq j\leq m$. The inner [bit-flip repetition code](../../../../../../bit-flip-repetition-code.md) has stabilizers

$$
S^Z_{i,j}=Z_{i,j}Z_{i,j+1},
\qquad 1\leq j<m,
$$

and logical operators $\overline X_i=\prod_{j=1}^mX_{i,j}$ and $\overline Z_i=Z_{i,1}$. Replacing each outer $X_i$ by $\overline X_i$ gives the outer stabilizers

$$
S^X_i=\prod_{j=1}^mX_{i,j}X_{i+1,j},
\qquad 1\leq i<n.
$$

This is the [surface code on a chain of spheres](../../../../../../surface-code-on-a-chain-of-spheres.md). The $n+1$ pole-touching points are vertices, and the $m$ longitudes on sphere $i$ are its qubit-carrying links. At an interior touching point, the star operator is exactly $S_i^X$. Each face between adjacent longitudes has the two-edge plaquette operator $Z_{i,j}Z_{i,j+1}$; only $m-1$ of the $m$ face operators on each sphere are independent.

Using the conventions of part a, logical operators are

$$
\boxed{
\overline Z=\prod_{j=1}^mX_{i,j},
\qquad
\overline X=\prod_{i=1}^nZ_{i,j}.}
$$

The first may be placed on any one sphere and is a dual equatorial cut crossing all $m$ longitude links. The second may use any fixed longitude and is a pole-to-pole path through all $n$ spheres. Multiplication by stabilizers deforms either representative without changing its logical action. Their minimum weights are $m$ and $n$, respectively, so the [distance of a stabilizer code](../../../../../../distance-of-a-stabilizer-code.md) is

$$
\boxed{d=\min(m,n).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
