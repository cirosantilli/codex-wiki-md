<h1 id="5/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Give the three [Hopf fibration](../../../../../../hopf-fibration.md) components coherent orientations, so their pairwise [linking numbers](../../../../../../linking-number.md) are one. In the [link exterior](../../../../../../link-exterior.md), their longitudes satisfy $[\lambda_i]=\sum_{j\ne i}\mu_j$. Filling along $p_i\mu_i+q_i\lambda_i$ imposes that relation on [first homology](../../../../../../first-homology.md). For the three rational coefficients the presentation matrix is

$$
M=\begin{pmatrix}1&2&2\\3&1&3\\5&5&1\end{pmatrix}.
$$

Its [determinant](../../../../../../determinant.md) is $30$, and the greatest common divisor of its two-by-two minors is one (for example, $-5$ and $-3$ occur). Its [Smith normal form](../../../../../../smith-normal-form.md) is $\operatorname{diag}(1,1,30)$, so

$$
\boxed{H_1(Z;\mathbb Z)\cong\mathbb Z/30\mathbb Z.}
$$

A nonzero rational coefficient with numerator one does not by itself make a multi-component surgery an [integral homology sphere](../../../../../../homology-sphere.md): the nonzero [linking numbers](../../../../../../linking-number.md) must be included.

For the integer filling, use the [Seifert fibered space](../../../../../../seifert-fibered-space.md) structure $P\times S^1$. Its central regular fiber is $h=abc$, and each preferred longitude is $h\mu_i^{-1}$. The three filling relations are consequently

$$
h=a^2,\qquad h=b,\qquad hc^4=1.
$$

Substituting $b=h$ into $abc=h$ gives $c=a^{-1}$. The remaining equations say $a^2=a^4$, hence $a^2=1$ and $h=1$. Thus its [fundamental group](../../../../../../fundamental-group.md) is cyclic of order two.

Geometrically, a filling coefficient $r$ attaches a [Seifert fibered space](../../../../../../seifert-fibered-space.md) solid torus with multiplicity $|r-1|$, the distance of $r\mu+\lambda$ from the regular fiber $\mu+\lambda$. The multiplicities are $2,1,4$; the middle filling creates no exceptional fiber. The result is a [Seifert fibered space](../../../../../../seifert-fibered-space.md) over the sphere with at most two exceptional fibers, hence a union of two [solid tori](../../../../../../solid-torus.md), or a [lens space](../../../../../../lens-space.md). A [lens space](../../../../../../lens-space.md) with fundamental group of order two is $L(2,1)$. Therefore

$$
\boxed{Y_{-1,0,5}\cong L(2,1)\cong\mathbb{RP}^3.}
$$

As a separate arithmetic check, the integer [surgery linking matrix](../../../../../../surgery-linking-matrix.md) has determinant $-2$, in agreement with its first homology of order two.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
