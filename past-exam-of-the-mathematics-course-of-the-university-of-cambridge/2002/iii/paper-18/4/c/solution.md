<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [root hyperplanes](../../../../../../root-hyperplane.md) are $x_1=0$, $x_2=0$, $x_1=x_2$ and $x_1=-x_2$. Their reflections are coordinate sign changes, coordinate interchange and a signed interchange. They generate all signed permutations of the two coordinates:

$$
\boxed{W\cong(\mathbb Z/2\mathbb Z)^2\rtimes S_2,\qquad |W|=8.}
$$

Geometrically this is the dihedral symmetry group of a square, with order eight. It preserves both the four short roots and the four long roots of the [B2 root system](../../../../../../b2-root-system.md).

Representatives in $SO(5)$ can be given explicitly. The matrix

$$
D_1=\operatorname{diag}(1,-1,1,1,-1)
$$

has determinant one and conjugates the first rotation block to its inverse, giving $(x_1,x_2)\mapsto(-x_1,x_2)$. The matrix $D_2=\operatorname{diag}(1,1,1,-1,-1)$ similarly reverses $x_2$. Flipping the fifth coordinate compensates for the determinant of the planar reflection.

The permutation matrix

$$
P=\begin{pmatrix}
0&0&1&0&0\\
0&0&0&1&0\\
1&0&0&0&0\\
0&1&0&0&0\\
0&0&0&0&1
\end{pmatrix}
$$

swaps the two coordinate planes. Its permutation is $(1\ 3)(2\ 4)$, so its determinant is also one. Conjugation gives $(x_1,x_2)\mapsto(x_2,x_1)$, the reflection in $x_1=x_2$. These elements normalize $T$, and $P,D_1$ generate all eight Weyl actions. For example, $PD_1$ induces $(x_1,x_2)\mapsto(x_2,-x_1)$, a quarter-turn, and $D_1D_2$ induces the half-turn. The representatives supply the specified reflections and their typical products inside the actual special orthogonal group.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
