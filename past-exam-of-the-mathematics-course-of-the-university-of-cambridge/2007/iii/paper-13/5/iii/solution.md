<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Harris theorem for square-lattice bond percolation](../../../../../../harris-theorem-for-square-lattice-bond-percolation.md) asserts $\theta(1/2)=0$, and hence $p_c\geq1/2$. Work in the dual [square lattice](../../../../../../square-lattice.md), declaring a dual bond open precisely when its primal bond is closed. At $p=1/2$ this is again independent [bond percolation](../../../../../../bond-percolation-split.md) of density one half.

Around a square centered at the origin place four dual rectangles of dimensions $6r$ by $2r$, one on each side, with overlap squares at the corners. Long crossings of all four must meet in the corner squares and their union contains a dual circuit surrounding the central square. The fixed-aspect crossing bound and the [Harris lemma](../../../../../../harris-inequality.md) give this dual barrier a [probability](../../../../../../probability.md) at least $\eta:=c_3^4>0$, independent of $r$.

Take geometrically increasing integer radii, for example with a factor of eight, and shift by half a lattice spacing to lie on the dual lattice. The four-rectangle annuli then have disjoint bond sets. Their barrier events are independent. An infinite primal open path from the origin would have to avoid every closed dual circuit, so the [independent annular barriers for percolation](../../../../../../independent-annular-barriers-for-percolation.md) give

$$
\mathbb P_{1/2}(|C_0|=\infty)\leq(1-\eta)^j\qquad\text{for every }j.
$$

Letting $j\to\infty$ proves

$$
\boxed{\theta(1/2)=0,\qquad\theta(p)=0\text{ for }p\leq1/2,\qquad p_c\geq1/2.}
$$

The extension to smaller $p$ follows by the [monotone coupling of Bernoulli percolation](../../../../../../monotone-coupling-of-bernoulli-percolation.md). Translation and a countable union also show that no infinite open cluster exists anywhere at $p=1/2$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
