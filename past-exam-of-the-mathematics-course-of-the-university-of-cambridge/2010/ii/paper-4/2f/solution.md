<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The fourth [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) is $T_4(x)=8x^4-8x^2+1$. Therefore take

$$
\boxed{p(x)=x^2-\frac18,\qquad \|x^4-p(x)\|_\infty=\frac18.}
$$

Indeed $x^4-p(x)=T_4(x)/8$, and $|T_4(x)|\le1$ on $[-1,1]$, as follows from $T_4(\cos\theta)=\cos4\theta$.

Here is a direct [Chebyshev alternation theorem](../../../../../equioscillation-theorem.md) argument proving optimality, without assuming the theorem. At the five ordered points

$$
-1,\quad-1/\sqrt2,\quad0,\quad1/\sqrt2,\quad1,
$$

the error $x^4-p(x)$ takes the alternating values $1/8,-1/8,1/8,-1/8,1/8$. If a [polynomial](../../../../../polynomial-split.md) $q$ of degree at most three had strictly smaller uniform error, then $q-p$ would have alternating strictly positive and strictly negative values at these points. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) would give a distinct root in each of the four intervening intervals. A nonzero [polynomial](../../../../../polynomial-split.md) of degree at most three cannot have four distinct roots. This contradiction proves the required minimax inequality.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
