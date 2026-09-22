<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Here a planar lattice means a [discrete subgroup](../../../../../discrete-subgroup.md) of the additive Euclidean plane; full rank is not required. Discreteness at zero gives an $\epsilon>0$ such that distinct lattice points are at least $\epsilon$ apart. Consequently every bounded set contains only finitely many lattice points, by placing disjoint small disks around them. If the group is zero, it has the stated one-generator form with $w=0$.

Otherwise choose a shortest nonzero lattice vector $w_1$. Every lattice point on its line is an integer multiple: subtract the nearest integer multiple of $w_1$ from a putative noninteger multiple to obtain a nonzero shorter vector, a contradiction. This already proves the one-generator case when all lattice points lie on that line.

For the remaining case choose the perpendicular orientation so that some point has positive height above the line of $w_1$. Reduce its parallel component modulo $w_1$ into $[0,|w_1|)$. Among reduced points of positive height there is a least height $d>0$. Indeed, heights tending to zero would give infinitely many points in a bounded strip, contrary to the finiteness just proved; bounded sets also ensure that a positive infimum is attained. Choose $w_2$ at height $d$.

Given any lattice vector $v$, subtract an integer multiple of $w_2$ so that its height lies in $[0,d)$, then reduce its parallel component modulo $w_1$. Minimality of $d$ forces the residual height to be zero, and the one-dimensional argument forces the residual to be an integer multiple of $w_1$. Therefore

$$
\boxed{\Lambda=\mathbb Zw_1+\mathbb Zw_2,\qquad w_1,w_2\text{ linearly independent}.}
$$

Together with the rank-one and zero cases this proves the [planar discrete-subgroup basis](../../../../../planar-discrete-subgroup-basis.md) assertion. Under the alternative convention that a Euclidean lattice must have full rank, only the two-generator case is called a lattice.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
