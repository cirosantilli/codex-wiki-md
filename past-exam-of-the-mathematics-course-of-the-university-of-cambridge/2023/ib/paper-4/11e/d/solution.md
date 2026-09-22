<h1 id="11e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [hyperboloid model](../../../../../../hyperboloid-model.md) with [Minkowski inner product](../../../../../../minkowski-inner-product.md)

$$
\langle x,y\rangle_M=-x_0y_0+x_1y_1+x_2y_2.
$$

Put the vertex with angle $\theta$ at $v=(1,0,0)$, and place the endpoints of its adjacent sides of lengths $a$ and $b$ at

$$
P=(\cosh a,\sinh a,0),
$$



$$
Q=(\cosh b,\sinh b\cos\theta,
\sinh b\sin\theta).
$$

The geodesic through $P$ perpendicular to $vP$ has spacelike unit normal

$$
n_P=(\sinh a,\cosh a,0),
$$

while the geodesic through $Q$ perpendicular to $vQ$ has spacelike unit normal

$$
n_Q=(\sinh b,\cosh b\cos\theta,
\cosh b\sin\theta).
$$

These two geodesics form the remaining two sides of the quadrilateral. Their angle equals the angle between their normals in the tangent plane at their intersection. The third right angle therefore gives

$$
0=\langle n_P,n_Q\rangle_M
=-\sinh a\sinh b+\cosh a\cosh b\cos\theta.
$$

Dividing by $\cosh a\cosh b$ proves the [Lambert quadrilateral identity](../../../../../../lambert-quadrilateral.md)

$$
\boxed{\cos\theta=\tanh a\tanh b}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
