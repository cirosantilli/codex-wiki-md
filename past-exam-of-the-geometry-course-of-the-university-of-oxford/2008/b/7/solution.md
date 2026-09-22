<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For a degree-$d$ nonconstant [holomorphic map](../../../../holomorphic-map.md) from a compact connected [Riemann surface](../../../../riemann-surfaces-split.md) of [genus](../../../../genus-of-a-surface.md) $g$ to the [projective line](../../../../projective-line.md), the [Riemann-Hurwitz formula](../../../../riemann-hurwitz-formula.md) is

$$
\boxed{2g-2=-2d+\sum_{p\in X}(e_p-1),}
$$

where $e_p$ is the [local degree](../../../../local-degree-of-a-continuous-map.md). A [meromorphic function](../../../../meromorphic-function.md) defines a map to the [sphere](../../../../sphere.md) by giving its ordinary finite values away from poles and value infinity at each pole. The reciprocal function is holomorphic in a neighborhood of a pole, proving holomorphicity there. For use in Riemann-Hurwitz the function must be nonconstant; a nonzero constant still defines a [holomorphic map](../../../../holomorphic-map.md), but of degree zero.

Let $X=\mathbb C/\Lambda$. The [double pole](../../../../double-pole.md) of $\wp$ gives a degree-two map to the [sphere](../../../../sphere.md). The [torus](../../../../torus.md) has [genus](../../../../genus-of-a-surface.md) one, so total ramification is four. One simple [ramification point](../../../../ramification-point-of-a-holomorphic-map.md) is zero, above infinity. At the three nonzero half-period classes $h_i$, evenness and periodicity give $\wp'(h_i)=0$. Each is a [ramification point](../../../../ramification-point-of-a-holomorphic-map.md) of [local degree](../../../../local-degree-of-a-continuous-map.md) two, and these account for all remaining ramification. Put $e_i=\wp(h_i)$. They are distinct, since a degree-two fiber cannot contain two points each of [local degree](../../../../local-degree-of-a-continuous-map.md) two.

At each $h_i$, $\wp-e_i$ has a double zero and $\wp'$ has a simple zero. Consequently the elliptic quotient

$$
R(z)=\frac{\wp'(z)^2}{(\wp(z)-e_1)(\wp(z)-e_2)(\wp(z)-e_3)}
$$

has removable singularities there and no zeros or poles elsewhere except possibly zero. Near zero, $\wp=z^{-2}+O(z^2)$ and $\wp'=-2z^{-3}+O(z)$, so $R\to4$. Thus $R$ is holomorphic on the compact [torus](../../../../torus.md) and constant, proving

$$
\boxed{\wp'^2=4(\wp-e_1)(\wp-e_2)(\wp-e_3).}
$$

**The printed additional requirement that all three $e_i$ be nonzero is false.** For the square lattice $\Lambda=\mathbb Z+i\mathbb Z$, invariance of the defining series under multiplication by $i$ gives $\wp(iz)=-\wp(z)$. At $h=(1+i)/2$, one has $ih=h-1$, so periodicity gives $\wp(h)=\wp(ih)=-\wp(h)$ and hence $\wp(h)=0$. This is one of the three branch values. Distinctness, which is all the cubic construction needs, remains valid.

Define

$$
\Phi(z)=[\wp(z):\wp'(z):1]\quad(z\notin\Lambda),\qquad\Phi(0)=[0:1:0].
$$

The image lies on $Y^2Z=4(X-e_1Z)(X-e_2Z)(X-e_3Z)$. Distinct roots make its affine part smooth, and the point at infinity is smooth because the derivative of its equation with respect to $Z$ is nonzero there. Near zero the projective coordinates $X/Y=\wp/\wp'\sim-z/2$ and $Z/Y=1/\wp'\sim-z^3/2$ extend holomorphically. Every finite $X/Z$ value has two preimages under $\wp$ except at a branch value. Evenness pairs those preimages as $z,-z$, and oddness of $\wp'$ distinguishes them unless they are the same half-period class. Therefore the two coordinates together give injectivity and reach both signs of $Y$, proving surjectivity onto the cubic. Thus **$\Phi$ is a bijective [holomorphic map](../../../../holomorphic-map.md) to a nonsingular cubic**, including when one branch value is zero.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
