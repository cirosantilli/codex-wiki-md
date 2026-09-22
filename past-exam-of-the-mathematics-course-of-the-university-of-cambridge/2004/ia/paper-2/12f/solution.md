<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Because the [events](../../../../../event.md) are pairwise [disjoint events](../../../../../disjoint-events.md), their count can only be zero or one. The [event](../../../../../event.md) that the count is zero is the [complement of an event](../../../../../complement-of-an-event.md) of their union. Finite additivity therefore gives

$$
\boxed{\mathbb P(N=0)=1-\mathbb P\left(\bigcup_{i=1}^r A_i\right)
=1-\sum_{i=1}^r\mathbb P(A_i).}
$$

Now use $N\geq1$ for the fixed number of independently located ships. Normalize the radius to one and write their positions as unit vectors $a_1,\ldots,a_N$. A point $x$ on the [sphere](../../../../../sphere.md) is reached by ship $i$ precisely when $a_i\cdot x>0$, so each ship reaches an open [hemisphere](../../../../../hemisphere.md). Coverage fails exactly when there is a unit vector $x$ with $a_i\cdot x\leq0$ for every $i$. Equivalently, all ship positions lie in some closed [hemisphere](../../../../../hemisphere.md).

With [probability](../../../../../probability.md) one no pair of ship vectors is antipodal and no three are linearly dependent: the exceptional choices lie on sets of zero surface area. For such a configuration, containment in a closed [hemisphere](../../../../../hemisphere.md) implies containment in an open [hemisphere](../../../../../hemisphere.md). To see this, choose its inward normal $u$, so $u\cdot a_i\geq0$. At most two vectors lie on its boundary. If there are two, their sum has positive dot product with each, since they are not antipodal; if there is one, use that vector itself. Perturb $u$ slightly in this direction. The boundary dot products become positive while all already positive dot products remain positive. Thus the strict and non-strict containment conditions have the same [probability](../../../../../probability.md) here.

Condition on the unoriented axes $\{a_i,-a_i\}$. Choose representatives $b_i$ by any fixed sign convention. By uniform sampling and [independence](../../../../../independent-random-variables.md), the actual positions are $a_i=\varepsilon_i b_i$ with $N$ [independent](../../../../../independent-random-variables.md) fair signs $\varepsilon_i\in\{-1,1\}$. Conditional on these axes, each of the $2^N$ sign choices has [probability](../../../../../probability.md) $2^{-N}$.

The [great circles](../../../../../great-circle.md) $b_i\cdot u=0$ partition the [sphere](../../../../../sphere.md) into $R_N=N(N-1)+2$ open regions. In each region the sign vector $\sigma(u)=(\operatorname{sgn}(b_i\cdot u))_i$ is constant. No sign vector labels two different regions: its strict inequalities define a convex cone, and normalized line segments within that cone connect any two points of its spherical section. The [regions of a general-position great-circle arrangement](../../../../../regions-of-a-general-position-great-circle-arrangement.md) therefore yield exactly $R_N$ realized sign vectors.

The chosen positions lie in an open [hemisphere](../../../../../hemisphere.md) if and only if some $u$ has $u\cdot a_i>0$ for every $i$, that is, $\varepsilon_i=\operatorname{sgn}(b_i\cdot u)$ for every $i$. Failure of coverage thus corresponds exactly to one of the $R_N$ realized sign choices. These choices are mutually exclusive [events](../../../../../event.md), each of [conditional probability](../../../../../conditional-probability.md) $2^{-N}$, so the first part applies:

$$
\mathbb P(\text{failure}\mid\text{axes})=\frac{R_N}{2^N}.
$$

The result is independent of the axes. Averaging gives the [coverage of a sphere by random open hemispheres](../../../../../coverage-of-a-sphere-by-random-open-hemispheres.md):

$$
\boxed{\mathbb P(\text{every point is reached})=1-\frac{N(N-1)+2}{2^N},\qquad N\geq1.}
$$

For $N=1,2,3$ this is zero; for $N=4$ it is $1/8$. If no ship lands, coverage has [probability](../../../../../probability.md) zero separately. The counting uses equiprobable orientation signs, not an assumption that the spherical regions have equal area.

## ↑ Ancestors (11)

1. [12F](../12f.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
