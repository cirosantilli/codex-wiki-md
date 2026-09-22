<h1 id="b/6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write the equation as $y^2=x^3-5x^2+4x$. Its [duplication formula](../../../../../elliptic-curve-group-law-from-riemann-roch.md) uses slope $m=(3x^2-10x+4)/(2y)$ and $x(2P)=m^2+5-2x$. At the three listed points the slopes are respectively $i$, $-1+i\sqrt3$, and $2+\sqrt3$. Substitution gives

$$
\boxed{2P_1=(0,0),\qquad2P_2=(1,0),\qquad2P_3=(4,0).}
$$

These are nonidentity points of order two, so each listed point has exactly order four.

For $p\ne2,3$ the three distinct [roots](../../../../../root-of-a-polynomial.md) zero, one and four give the full two-[torsion subgroup](../../../../../torsion-subgroup.md) of order four over $\mathbb F_p$. At least one of $-1,3,-3$ is a square: if neither of the first two is, their product is. If $-1$ is a square, the first listed point exists over the [field](../../../../../field.md). If three is a square, the third exists. If $-3$ is a square, the second can be written $(1-\sqrt{-3},3+\sqrt{-3})$ and exists without requiring the two separate square [roots](../../../../../root-of-a-polynomial.md). The duplication computations remain valid after reduction; their ordinates do not vanish unless $p=2$ or three. Thus a rational [two-torsion](../../../../../2-torsion.md) point has a half over the [field](../../../../../field.md). Together with a different [two-torsion](../../../../../2-torsion.md) point this generates a [subgroup](../../../../../subgroup.md) of order eight. Consequently $\boxed{8\mid\#E(\mathbb F_p)}$ for every stated [prime](../../../../../prime-number-split.md).

Over the rationals there are already four [two-torsion](../../../../../2-torsion.md) points, including the identity. Counting at five gives eight points: the abscissas zero, one and four give one ordinate each, two and three give two each, and there is the identity. Thus [rational torsion](../../../../../torsion-subgroup.md) has order dividing eight.

There are no [rational points](../../../../../rational-point.md) of order four. For a curve $y^2=\prod_j(x-e_j)$, translating $e_i$ to zero and using the [duplication formula](../../../../../elliptic-curve-group-law-from-riemann-roch.md) shows that a half of $(e_i,0)$ must satisfy $(x-e_i)^2=(e_i-e_j)(e_i-e_k)$. For the three [roots](../../../../../root-of-a-polynomial.md) here, the candidate abscissas are $\pm2$, $1\pm\sqrt{-3}$, and $4\pm2\sqrt3$. The last two pairs are nonrational; at $x=2,-2$ the ordinate squares are $-4,-36$, also impossible over $\mathbb Q$. A group of order eight containing this two-[torsion subgroup](../../../../../torsion-subgroup.md) would contain an element of order four, because an [elliptic curve](../../../../../elliptic-curve.md) has only four points killed by two. Hence

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}\cong C_2\times C_2,\qquad\#E(\mathbb Q)_{\mathrm{tors}}=4.}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
