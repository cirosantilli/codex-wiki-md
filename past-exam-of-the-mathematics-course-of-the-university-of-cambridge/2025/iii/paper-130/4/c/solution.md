<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\rho^2=28-28\sqrt5/5$ and, for $j\in\mathbb Z/30\mathbb Z$, define

$$
v_j=
\left(
5\cos\frac{j\pi}{3},
5\sin\frac{j\pi}{3},
\rho\cos\frac{4j\pi}{5},
\rho\sin\frac{4j\pi}{5}
\right).
$$

The shift $v_j\mapsto v_{j+1}$ is an [isometry](../../../../../../isometry.md) acting transitively on the finite set $V=\{v_j\}$, so $V$ is a [cyclic transitive point set](../../../../../../cyclic-transitive-point-set.md) and hence a [Euclidean Ramsey set](../../../../../../euclidean-ramsey-set.md) by the [Kriz theorem for cyclic transitive point sets](../../../../../../kriz-theorem-for-cyclic-transitive-point-sets.md).

For every $j,k$,

$$
\lVert v_{j+k}-v_j\rVert^2
=50\left(1-\cos\frac{k\pi}{3}\right)
+\left(56-\frac{56\sqrt5}{5}\right)
\left(1-\cos\frac{4k\pi}{5}\right).
$$

For $k=1,5,11,15,4,14$, these squared distances are respectively

$$
81,25,81,100,131,131.
$$

Consequently $v_0,v_1,v_{26},v_{15}$, in that order, have consecutive side lengths $9,5,9,10$ and equal diagonals $\sqrt{131}$. This is an isometric copy of the required isosceles [trapezium](../../../../../../trapezoid.md). Since every monochromatic copy of $V$ contains this four-point subset, the trapezium is Euclidean Ramsey.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
