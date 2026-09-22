<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [Newton's method](../../../../../newton-s-method-in-optimization.md) to $F(t)=1-3\sin t/2-\sin^3t/3$. The derivative in part (a) gives

$$
\boxed{t_{k+1}=t_k+\frac{1-\frac32\sin t_k-\frac13\sin^3t_k}{\cos t_k\left(\frac32+\sin^2t_k\right)}.}
$$

Choose a starting point near a desired root, such as $t_0=0.6$ for the root in $(0,\pi/2)$; do not divide when $\cos t_k=0$. On $(0,\pi/2)$, $F$ is strictly decreasing and changes sign between its endpoints, so the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives exactly one root there. Its derivative is nonzero, giving the usual local convergence of [Newton's method](../../../../../newton-s-method-in-optimization.md). The [periodic function](../../../../../periodic-function.md) has other roots; the iteration does not impose global uniqueness or convergence from every starting value.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
