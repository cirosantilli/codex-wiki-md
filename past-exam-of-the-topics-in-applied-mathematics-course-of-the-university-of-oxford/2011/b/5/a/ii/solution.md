<h1 id="b/5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Follow a perturbation through one complete circuit. The chain rule gives

$$
\delta x_k=M\delta x_0+O(\|\delta x_0\|^2),\qquad M=Df(x_{k-1})\cdots Df(x_1)Df(x_0).
$$

After $m$ circuits the linear perturbation is $M^m\delta x_0$. With distinct [eigenvalues](../../../../../../eigenvalue.md), the [eigenvectors](../../../../../../eigenvector.md) span over the complex numbers, and each component is multiplied by $\lambda_j^m$. Thus the [periodic orbit](../../../../../../periodic-orbit.md) is linearly asymptotically stable exactly when

$$
\boxed{|\lambda_j(M)|<1\quad\text{for every }j.}
$$

These are the orbit's discrete [Floquet multipliers](../../../../../../floquet-multiplier.md). Any modulus greater than one causes instability; a unit modulus prevents decay in the linear system, and nonlinear stability then needs further analysis. The finitely many intermediate [derivative](../../../../../../derivative.md) factors do not affect convergence to zero between complete circuits.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
