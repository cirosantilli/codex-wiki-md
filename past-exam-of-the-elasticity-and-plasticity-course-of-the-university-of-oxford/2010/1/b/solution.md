<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A Cartesian [Cartesian second-rank tensor](../../../../cartesian-second-rank-tensor.md) has components transforming under a constant orthogonal change of axes as

$$
\boxed{T'_{ij}=p_{ia}p_{jb}T_{ab},\qquad T'=PTP^T.}
$$

Here $\mathbf X'=P\mathbf X$ and $\mathbf u'=P\mathbf u$. By the [chain rule](../../../../chain-rule.md) and orthogonality,

$$
\frac{\partial u_i'}{\partial X_j'}
=p_{ia}\frac{\partial u_a}{\partial X_b}\frac{\partial X_b}{\partial X_j'}
=p_{ia}p_{jb}\frac{\partial u_a}{\partial X_b}.
$$

Thus the [displacement](../../../../displacement.md) [gradient](../../../../gradient.md) is a [Cartesian second-rank tensor](../../../../cartesian-second-rank-tensor.md). Its symmetric part transforms in the same way:

$$
e'_{ij}=\frac12p_{ia}p_{jb}
\left(\frac{\partial u_a}{\partial X_b}+\frac{\partial u_b}{\partial X_a}\right)
=p_{ia}p_{jb}e_{ab}.
$$

Hence **the [infinitesimal strain tensor](../../../../infinitesimal-strain-tensor.md) is also second-rank**. This is a passive coordinate rotation, under which both reference and spatial coordinates rotate; it does not assert finite-[deformation](../../../../deformation-mechanics.md) frame indifference of the linearized strain formula.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
