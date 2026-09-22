<h1 id="continuous-mathematics/5/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For a generic integrand in 20 dimensions, [Monte Carlo integration](../../../../../../../monte-carlo-integration.md) gives [root mean square](../../../../../../../root-mean-square.md) error $O(N^{-1/2})$, whereas [tensor-product quadrature](../../../../../../../tensor-product-quadrature.md) with [composite Simpson's rule](../../../../../../../composite-simpson-s-rule.md) gives only $O(N^{-4/20})=O(N^{-1/5})$. One can sample uniformly in the [Euclidean unit ball](../../../../../../../euclidean-unit-ball.md), for example by an independent uniform direction and radius $U^{1/20}$ with $U$ uniform on $[0,1]$.

For this particular integrand, the most efficient elementary choice uses [radial integration over a ball](../../../../../../../radial-integration-over-a-ball.md) first. The area of the unit 19-sphere is $2\pi^{10}/9!$, as follows from the [volume of an n-ball](../../../../../../../volume-of-an-n-ball.md). Hence

$$
I=\frac{2\pi^{10}}{9!}\int_0^1 e^{r^2}r^{19}\,dr=\frac{\pi^{10}}{9!}\int_0^1 e^t t^9\,dt.
$$

The reduced integrand is smooth. Apply [composite Simpson's rule](../../../../../../../composite-simpson-s-rule.md) to obtain **$O(N^{-4})$** deterministic error in [big O notation](../../../../../../../big-o-notation.md), with one original radial integrand evaluation per node. If the selection is restricted to direct multidimensional methods, **[Monte Carlo integration](../../../../../../../monte-carlo-integration.md) with $O(N^{-1/2})$ [root mean square](../../../../../../../root-mean-square.md) error** is the appropriate choice.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Continuous mathematics](../../../../continuous-mathematics.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
