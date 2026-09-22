<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\sigma$ denote [surface measure on a sphere](../../../../../surface-measure-on-a-sphere.md) on $S^2$ and $\nu$ volume measure on the unit ball. The [Poisson mapping theorem](../../../../../poisson-mapping-theorem.md) can be proved directly here: counts of image points in disjoint sets are counts of the original process in their disjoint preimages. They are therefore [independent](../../../../../independent-random-variables.md) Poisson variables, and their means are the volumes of those preimages.

For the radius map, a [measurable](../../../../../measurability.md) set $A\subset[0,1]$ has mean

$$
\boxed{\nu_1(A)=\int_A4\pi r^2\,dr,\qquad
\nu_1([0,a])=\frac{4\pi a^3}{3}\quad(0\le a\le1).}
$$

This follows from [spherical coordinates](../../../../../spherical-coordinate-system.md) or by subtracting concentric-ball volumes. The disjoint-preimage argument proves that the radius image is a [Poisson process](../../../../../poisson-process.md) with this [mean measure of a point process](../../../../../intensity-measure-of-a-point-process.md). There is no mass at zero or at one.

The original process has no point at the origin [almost surely](../../../../../almost-sure-convergence.md), since its mean count there is zero. Thus division by $r$ in the direction map is well-defined [almost surely](../../../../../almost-sure-convergence.md). For a [measurable](../../../../../measurability.md) surface set $C\subset S^2$, [spherical coordinates](../../../../../spherical-coordinate-system.md) give

$$
\boxed{\nu_2(C)=\int_C\int_0^1r^2\,dr\,\sigma(d\omega)=\frac{\sigma(C)}3.}
$$

Again disjoint surface sets have disjoint cone preimages, giving the required [independent](../../../../../independent-random-variables.md) Poisson counts. Both [pushforward measures](../../../../../pushforward-measure.md) are diffuse, so there are [almost surely](../../../../../almost-sure-convergence.md) no image collisions; they describe the indicated point sets as well as [counting measures](../../../../../counting-measure.md).

**The two image processes are not [independent](../../../../../independent-random-variables.md).** They have exactly the same total number of points,

$$
N=\Pi_1([0,1])=\Pi_2(S^2)=\Pi(B)\sim\operatorname{Pois}(4\pi/3).
$$

Indeed,

$$
\mathbb P(\Pi_1=\varnothing,\Pi_2=\varnothing)=e^{-4\pi/3}
\ne e^{-8\pi/3}
=\mathbb P(\Pi_1=\varnothing)\mathbb P(\Pi_2=\varnothing).
$$

This alone disproves process [independence](../../../../../independent-random-variables.md).

More generally, split the original points into those whose radius lies in $A$ and direction lies in $C$, those satisfying only the first condition, and those satisfying only the second. Counts in these three disjoint regions are [independent](../../../../../independent-random-variables.md). The count shared by both images is Poisson with mean $\sigma(C)\int_A r^2dr$, so

$$
\operatorname{Cov}\bigl(\Pi_1(A),\Pi_2(C)\bigr)=\sigma(C)\int_A r^2\,dr.
$$

The fact that [Poisson polar projections share their total count](../../../../../poisson-polar-projections-share-their-total-count.md) explains the dependence despite the product polar intensity $r^2dr\,\sigma(d\omega)$. Conditional on $N$, the points are [independent](../../../../../independent-random-variables.md) uniform samples from the ball. Their radius density is $3r^2$ and their direction law is $\sigma/(4\pi)$, independently for each point. Thus the two image configurations are [independent](../../../../../independent-random-variables.md) conditional on $N$; unconditionally the shared nonconstant count couples them.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
