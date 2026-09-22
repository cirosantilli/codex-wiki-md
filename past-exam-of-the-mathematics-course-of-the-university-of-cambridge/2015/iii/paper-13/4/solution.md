<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For each element $x$ of the [product set](../../../../../product-set.md) $A\cdot B$, let $s_x$ count its representations as $ab$ with $(a,b)\in A\times B$. The ratio equality $a/b=c/d$ is equivalent to $ad=cb$. Swapping the two $B$ coordinates is a [bijection](../../../../../bijection.md) between the ratio-equality quadruples and the equal-product quadruples. Therefore the [multiplicative energy](../../../../../multiplicative-energy.md) satisfies

$$
E(A,B)=\sum_{x\in A\cdot B}s_x^2,\qquad
\sum_{x\in A\cdot B}s_x=|A||B|.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives **the energy lower bound**:

$$
\boxed{E(A,B)\geq\frac{|A|^2|B|^2}{|A\cdot B|}.}
$$

For the upper bound, place the [Cartesian product](../../../../../cartesian-product.md) $P=A\times B$ in the strictly positive quadrant. For every occupied [Euclidean ray](../../../../../euclidean-ray.md) from the origin let $P_\lambda$ be its points and $r_\lambda=|P_\lambda|$. The slope is $\lambda=b/a$, so

$$
E(A,B)=\sum_\lambda r_\lambda^2,\qquad 1\leq r_\lambda\leq |B|.
$$

Take $\log$ to be the [natural logarithm](../../../../../natural-logarithm.md) and put $L=\lceil\log|B|\rceil\geq1$, using the non-triviality assumption $|B|\geq2$. Partition the possible occupancies into $L$ classes: $[e^j,e^{j+1})$ for $0\leq j<L-1$, and $[e^{L-1},|B|]$ for the last class. This last closed endpoint ensures that the partition works even when the top endpoint is attained. Within each class the ratio of any two occupancies is at most $e$.

Fix one class and order its occupied [Euclidean rays](../../../../../euclidean-ray.md) by increasing slope, with occupancies $r_1,\ldots,r_t$. Write $S=|A+A||B+B|$, the [cardinality](../../../../../cardinality.md) of $(A+A)\times(B+B)$. If $t=1$, then $r_1^2\leq|A||B|\leq S$, since adding any fixed element gives an [injection](../../../../../injective-function.md) of $A$ into its [sumset](../../../../../sumset.md) $A+A$, and similarly for $B$.

If $t\geq2$, the sums $P_i+P_{i+1}$ contain exactly $r_ir_{i+1}$ different points, by [injectivity of sums on two distinct rays](../../../../../injectivity-of-sums-on-two-distinct-rays.md). Indeed, the two direction vectors are [linearly independent](../../../../../linear-independence.md), so the [coefficients](../../../../../coefficient.md) of a sum uniquely recover its two summands. Positivity puts every sum strictly inside the [open planar sector](../../../../../open-planar-sector.md) between those two [Euclidean rays](../../../../../euclidean-ray.md). The sectors between successive selected [Euclidean rays](../../../../../euclidean-ray.md) are disjoint, even if there are additional unselected rays between them. All these sums belong to $(A+A)\times(B+B)$, and hence

$$
S\geq\sum_{i=1}^{t-1}r_ir_{i+1}.
$$

For neighbouring occupancies their ratio lies between $e^{-1}$ and $e$, so

$$
r_i^2+r_{i+1}^2\leq(e+e^{-1})r_ir_{i+1}<4r_ir_{i+1}.
$$

Summing covers every $r_i^2$ at least once, and gives $\sum_i r_i^2\leq4S$. The same bound holds for empty or singleton classes by the preceding observations. Adding over the $L$ classes proves the [multiplicative energy sumset bound](../../../../../multiplicative-energy-sumset-bound.md) $E(A,B)\leq4LS$. Combining both bounds yields **the sum-product conclusion**:

$$
\boxed{\frac{|A|^2|B|^2}{4\lceil\log|B|\rceil}
\leq |A\cdot B|\,|A+A|\,|B+B|.}
$$

If instead $\log$ is interpreted as base two, use the same $L=\lceil\log_2|B|\rceil$ occupancy classes with $2$ in place of $e$; $2+2^{-1}<4$ proves that convention as well. Positivity is essential to the sector argument.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
