<h1 id="7e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Centre the cube at the origin with faces having normals $\pm e_1,\pm e_2,\pm e_3$. Every rotational symmetry fixes the centre and permutes these normals, so its [rotation matrix](../../../../../../rotation-matrix.md) is a [signed permutation matrix](../../../../../../signed-permutation-matrix.md) of [determinant](../../../../../../determinant.md) one. Conversely any such [matrix](../../../../../../matrix.md) permutes the cube’s coordinates up to signs and preserves the cube. For each of $3!$ coordinate [permutations](../../../../../../permutation.md), four of the eight choices of signs give [determinant](../../../../../../determinant.md) one. Consequently the [rotational symmetry group of a cube](../../../../../../rotational-symmetry-group-of-a-cube.md) has

$$
\boxed{|H|=3!\,2^2=24.}
$$

This counts the rotations directly, without an unverified stabilizer calculation. The TeX’s $2^k$ is damaged transcription: the PDF prints 24.

Let $X$ be the $3^6$ face colourings. A colouring fixed by a rotation must be constant on each [permutation cycle](../../../../../../permutation-cycle.md) of faces, giving $3^c$ fixed colourings if the rotation has $c$ face cycles. The rotation types are:

| Rotation | Number | Face cycle type | Fixed colourings |
| --- | --- | --- | --- |
| Identity | 1 | $1^6$ | $3^6$ |
| Quarter-turn about opposite face centres | 6 | $1^2 4$ | $3^3$ |
| Half-turn about opposite face centres | 3 | $1^2 2^2$ | $3^4$ |
| Half-turn about opposite edge midpoints | 6 | $2^3$ | $3^3$ |
| Third-turn about opposite vertices | 8 | $3^2$ | $3^2$ |

There are three face axes, each with two quarter-turns and one half-turn; six edge axes, each with one half-turn; and four vertex axes, each with two nonidentity third-turns. These rotations are distinct and, with the identity, total 24, so the table is exhaustive. Face-axis rotations fix their two axial faces; the remaining four faces cycle or pair. Edge half-turns pair all faces, while vertex third-turns form two triples.

[Burnside lemma](../../../../../../burnside-s-lemma.md) now gives

$$
\boxed{|X/H|=\frac{3^6+6\cdot3^3+3\cdot3^4+6\cdot3^3+8\cdot3^2}{24}=57.}
$$

The three colours are labelled, [orthogonal reflections](../../../../../../reflection-in-a-hyperplane.md) are excluded, and no condition requires every colour to appear.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7E](../../7e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
