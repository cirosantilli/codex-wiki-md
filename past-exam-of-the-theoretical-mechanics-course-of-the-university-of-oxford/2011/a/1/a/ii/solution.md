<h1 id="a/1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define $\sigma_{ij}=\mathbf e_i\cdot\mathbf t(\mathbf e_j)$: the second index labels the normal direction of a coordinate face, and the first labels the [force](../../../../../../force-split.md) component. These nine entries form the [Cauchy stress tensor](../../../../../../cauchy-stress-tensor.md).

Take a small tetrahedron with oblique face of [area](../../../../../../surface-area.md) $S$ and outward normal $\mathbf n$. First suppose $n_j>0$; its other three faces have normals $-\mathbf e_j$ and areas $S_j=n_jS$, by [orthogonal](../../../../../../orthogonal-vectors.md) projection of the oblique face. The total surface [force](../../../../../../force-split.md) is

$$
S\mathbf t(\mathbf n)+\sum_jS_j\mathbf t(-\mathbf e_j).
$$

If its linear size is $\ell$, its inertia is $O(\ell^3)$ while its surface [forces](../../../../../../force-split.md) are $O(\ell^2)$. Divide the [momentum](../../../../../../momentum-split.md) balance by $S$ and shrink the tetrahedron to the point. Smoothness of the stress and the odd-normal relation then give $\mathbf t(\mathbf n)=\sum_jn_j\mathbf t(\mathbf e_j)$. Choosing coordinate faces with the appropriate reversed normals gives the same identity in the other octants. In components,

$$
\boxed{\mathbf t(\mathbf n)=\sum_{i,j}\mathbf e_i\sigma_{ij}n_j=\boldsymbol\sigma\mathbf n.}
$$

The face-[area](../../../../../../surface-area.md) relations used are exactly $S_j=|n_j|S$, with each coordinate face oriented opposite the corresponding component of the oblique normal.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
