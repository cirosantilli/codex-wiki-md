<h1 id="11d/solution">Solution</h1>

↑ **Parent:** [11D](../11d.md)

Uniform area density in the unit disk is $1/\pi$. The [polar coordinates](../../../../../polar-coordinates.md) Jacobian gives the joint density

$$
f_{R,\Theta}(r,\theta)
=\frac r\pi
=\left(2r\right)\left(\frac1{2\pi}\right),
\qquad
0\leq r\leq1,\quad0\leq\theta<2\pi.
$$

Thus the coordinates are independent and the [uniform random point in a disk](../../../../../uniform-random-point-in-a-disk.md) has

$$
\boxed{
f_R(r)=2r\mathbf1_{[0,1]}(r),
\qquad
f_\Theta(\theta)=\frac1{2\pi}\mathbf1_{[0,2\pi)}(\theta)}.
$$

For independent points $A,B$, the area of triangle $OAB$ is

$$
\frac12R_AR_B|\sin(\Theta_A-\Theta_B)|.
$$

Now

$$
\mathbb ER=\int_0^1 2r^2\,dr=\frac23,
\qquad
\mathbb E|\sin(\Theta_A-\Theta_B)|=\frac2\pi.
$$

Independence therefore gives

$$
\boxed{\mathbb E\,\operatorname{Area}(OAB)=\frac4{9\pi}}.
$$

Conditioned on $A,B$, the probability that $C$ lies inside $OAB$ is its area divided by the disk area $\pi$. Hence

$$
\boxed{\mathbb P(C\in\triangle OAB)=\frac4{9\pi^2}}.
$$

Four points in general position fail to form a convex quadrilateral exactly when one lies inside the triangle formed by the other three. Each of $A,B,C$ lies inside the triangle formed by $O$ and the other two with probability $4/(9\pi^2)$, and these three events are disjoint. The remaining possibility is that $O$ lies inside $ABC$. By [origin in a triangle of three radial random points](../../../../../origin-in-a-triangle-of-three-radial-random-points.md), this has probability $1/4$. Therefore

$$
\boxed{
\mathbb P(O,A,B,C\text{ form a convex quadrilateral})
=1-\frac14-\frac{4}{3\pi^2}
=\frac34-\frac4{3\pi^2}}.
$$

## ↑ Ancestors (10)

1. [11D](../11d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
