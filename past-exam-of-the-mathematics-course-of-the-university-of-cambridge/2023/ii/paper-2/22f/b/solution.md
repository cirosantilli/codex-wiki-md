<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here “isometry” is used in the standard [Mazur-Ulam theorem](../../../../../../mazur-ulam-theorem.md) sense of a surjective distance-preserving map. Surjectivity is needed; a merely distance-preserving embedding need not preserve midpoints, as shown by a [nonsurjective isometry need not preserve midpoints](../../../../../../nonsurjective-isometry-need-not-preserve-midpoints.md).

Distance preservation and surjectivity give

$$
u(S_1^{vw})=S_1^{u(v)u(w)}.
$$

Assume inductively that

$$
u(S_{n-1}^{vw})=S_{n-1}^{u(v)u(w)}.
$$

Then the two sets have the same diameter, and the universal distance condition defining the next set transfers through the bijection $u$. Hence

$$
u(S_n^{vw})=S_n^{u(v)u(w)}
$$

for every $n$.

Because $u$ is injective, it also preserves the intersection of this nested family. Part (a) therefore gives

$$
\left\{
u\left(\frac{v+w}{2}\right)
\right\}
=u\left(\bigcap_{n\geq1}S_n^{vw}\right)
=\bigcap_{n\geq1}S_n^{u(v)u(w)}
=\left\{
\frac{u(v)+u(w)}2
\right\}.
$$

Thus

$$
\boxed{
u\left(\frac{v+w}{2}\right)
=\frac{u(v)+u(w)}2.
}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
