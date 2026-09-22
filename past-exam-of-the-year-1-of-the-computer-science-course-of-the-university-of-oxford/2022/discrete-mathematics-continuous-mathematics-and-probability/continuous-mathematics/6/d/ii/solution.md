<h1 id="continuous-mathematics/6/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [diagonal reduction in a two-variable Newton iteration](../../../../../../../diagonal-reduction-in-a-two-variable-newton-iteration.md), $y_n=x_n$ for $n\ge1$. Put $e_n=x_n-1$. Direct factorization gives the exact [Newton map in optimization](../../../../../../../newton-map-in-optimization.md) error identity

$$
e_{n+1}=\frac{2x_n^3-(3x_n^2-1)}{3x_n^2-1}=e_n^2\frac{2x_n+1}{3x_n^2-1}.
$$

The assumed convergence $x_n\to1$ makes the final factor tend to $3/2$, so it is bounded for all sufficiently large $n$. Hence $|e_{n+1}|\le C|e_n|^2$. For the [Euclidean norm](../../../../../../../euclidean-norm.md) error $E_n=\|(x_n,y_n)-(1,1)\|=\sqrt2|e_n|$, this becomes **$E_{n+1}\le(C/\sqrt2)E_n^2$**, proving [quadratic convergence](../../../../../../../quadratic-convergence.md). Unless the exact limit is reached in finitely many steps, $E_{n+1}/E_n^2\to3/(2\sqrt2)$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [6](../../../6.md)
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
