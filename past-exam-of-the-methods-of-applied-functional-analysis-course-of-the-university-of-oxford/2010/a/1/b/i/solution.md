<h1 id="a/1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $a(v,w)=\int_\Omega a\nabla v\cdot\nabla w$ and $A[v]=a(v,v)$. The admissible set is the closed [affine subspace](../../../../../../affine-subspace.md) $H_g^1=g+H_0^1$. Symmetry of the coefficient matrix gives

$$
A[u+t\varphi]=A[u]+2t\,a(u,\varphi)+t^2A[\varphi],\qquad\varphi\in H_0^1.
$$

If $u$ minimizes the energy, its [first variation](../../../../../../first-variation.md) vanishes: differentiating at $t=0$ gives $a(u,\varphi)=0$. Hence $u$ is a [weak solution](../../../../../../weak-solution.md).

Conversely, if $u$ is a [weak solution](../../../../../../weak-solution.md), every admissible $v$ has $v-u\in H_0^1$ and therefore

$$
A[v]=A[u]+2a(u,v-u)+A[v-u]=A[u]+A[v-u]\geq A[u],
$$

by [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md). This is the [Dirichlet principle](../../../../../../dirichlet-principle.md) for the stated symmetric energy.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
