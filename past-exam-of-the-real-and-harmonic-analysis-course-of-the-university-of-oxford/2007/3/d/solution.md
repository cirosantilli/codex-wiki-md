<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $L_\xi(f)=\lim_NA_N(f)$. Limits preserve [linearity](../../../../linearity.md) and [positivity](../../../../positivity-linear-maps.md), and $|L_\xi(f)|\leq\|f\|_\infty$, $L_\xi(1)=1$. The [Riesz-Markov-Kakutani representation theorem](../../../../riesz-markov-kakutani-representation-theorem.md) supplies a unique Radon [probability measure](../../../../probability-measure.md) $\mu^\xi$. By its definition,

$$
\int f\,d\mu_N^\xi\longrightarrow\int f\,d\mu^\xi\quad(f\in C(\mathbb T)),
$$

which is exactly weak-star convergence in $C(\mathbb T)'$.

If $\xi/(2\pi)=p/q$ in lowest terms, the orbit has exactly $q$ points. Averaging a periodic sequence gives

$$
\boxed{\mu^\xi=\frac1q\sum_{r=0}^{q-1}\delta_{e^{ir\xi}}.}
$$

This includes $q=1$. If $\xi/\pi$ is irrational, then $e^{ik\xi}\ne1$ for every nonzero integer $k$. The preceding calculation gives $L_\xi(z^k)=0$ for $k\ne0$ and $L_\xi(1)=1$, exactly the integrals against normalized [Haar measure](../../../../haar-measure.md) $m$. [Density](../../../../density.md) of [trigonometric polynomials](../../../../trigonometric-polynomial.md) implies equality on all [continuous functions](../../../../continuous-function.md), and uniqueness gives

$$
\boxed{\mu^\xi=m\quad\text{when }\xi/\pi\text{ is irrational}.}
$$

These are the periodic-orbit and irrational-rotation cases of [equidistribution](../../../../equidistributed-sequence.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
