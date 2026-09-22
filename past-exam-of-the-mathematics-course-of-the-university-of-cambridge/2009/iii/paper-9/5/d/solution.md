<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [strong maximum principle for subharmonic functions](../../../../../../strong-maximum-principle-for-subharmonic-functions.md) states that an upper semicontinuous subharmonic function on a connected open set which attains its finite global maximum at an interior point is constant. In particular this holds for a harmonic function; negating the function gives the corresponding minimum principle for superharmonic functions.

Let the maximum be $M$, attained at $x_0$. For every sufficiently small ball centered at $x_0$, the [mean value inequality](../../../../../../mean-value-inequality.md) gives

$$
M=u(x_0)\leq\frac1{|B_r|}\int_{B_r(x_0)}u\leq M.
$$

Therefore its average equals $M$. If some point in the ball had value less than $M$, [upper semicontinuity](../../../../../../upper-semicontinuity.md) would give an open neighborhood where $u\leq M-\eta$ for some $\eta>0$. That positive-measure neighborhood would make the average strictly less than $M$, a contradiction. Thus $u=M$ throughout a neighborhood of $x_0$.

The same argument at each maximizing point shows that $\{u=M\}$ is open; it is also closed relative to the domain by upper semicontinuity. It is nonempty, so connectedness forces it to be the whole domain. Without connectedness, constancy is only guaranteed on the component containing the maximizing point.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
