<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

A parametrization is $X(\theta,z)=(\cosh z\cos\theta,\cosh z\sin\theta,z)$. It gives a [homeomorphism](../../../../../homeomorphism.md) $S^1\times\mathbb R\to S$, with inverse obtained from the height and angular position. Its [first fundamental form](../../../../../first-fundamental-form.md) is

$$
ds^2=\cosh^2z\,(d\theta^2+dz^2).
$$

For a surface of revolution with radius $r(z)$, the [Gaussian curvature](../../../../../gaussian-curvature.md) is $-r''/[r(1+r'^2)^2]$. Thus **$\boxed{K=-\operatorname{sech}^4z<0}$**. The waist $z=0$ is a closed [geodesic](../../../../../geodesic.md): $\Gamma^z_{\theta\theta}=-\tanh z$ vanishes there, and $\theta$ can be parametrized at constant speed.

For the [uniqueness of a closed geodesic on a negatively curved cylinder](../../../../../uniqueness-of-a-closed-geodesic-on-a-negatively-curved-cylinder.md), use [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) with piecewise geodesic boundary:

$$
\int_DK\,dA+\sum_j(\pi-\alpha_j)=2\pi\chi(D).
$$

A geodesic disk with smooth boundary would require curvature integral $2\pi$. A disk bounded by a geodesic monogon would require $\pi+\alpha>0$, and a geodesic bigon would require $\alpha+\beta>0$. All are impossible when $K<0$.

Here is the topological reduction needed to apply this observation without assuming simplicity. Lift a closed geodesic to the universal covering plane of the cylinder. A self-intersection of its lift supplies an innermost monogon by the [Jordan curve theorem](../../../../../jordan-curve-theorem.md), so the lift is embedded. A contractible closed geodesic would similarly supply a geodesic disk or monogon, so its winding number is nonzero. Its lift is consequently a proper line, invariant under a nonzero power of the deck translation. Two distinct translates of that line cannot intersect: periodicity would repeat an intersection, and innermost arcs between intersections would bound a bigon. The disjoint translates are ordered transversely, with the deck translation preserving that order. A finite cyclic permutation of this ordered family is impossible, so the lift is invariant under the primitive deck translation too. Thus the original geodesic has a simple image and is at most a repeated traversal of it.

Likewise two distinct simple essential closed geodesics cannot intersect: their periodic lifts would produce a bigon. If disjoint, the [Jordan curve theorem](../../../../../jordan-curve-theorem.md) on the cylinder says they bound a compact annulus. Its two boundaries have zero [geodesic curvature](../../../../../geodesic-curvature.md) and $\chi=0$, so Gauss-Bonnet gives $\int K\,dA=0$, again impossible. Therefore **there is at most one closed geodesic image**. Reparametrizations, reversed orientation and multiple traversals are understood to describe the same geometric geodesic.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
