<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the usual [inner product](../../../../inner-product-split.md) $\langle u,v\rangle=\int_0^1\overline u v\,dx$. Moving four [derivatives](../../../../derivative.md) by [integration by parts](../../../../integration-by-parts.md) leaves $L^*=D^4+1$ and gives the fourth-order boundary identity

$$
\langle u,Lv\rangle-\langle Lu,v\rangle
=\left[\overline u v'''-\overline {u'}v''+\overline {u''}v'-\overline {u'''}v\right]_0^1.
$$

Thus the differential expression is formally [self-adjoint](../../../../self-adjoint-operator.md). If both [functions](../../../../function-split.md) satisfy the [clamped boundary conditions](../../../../clamped-boundary-condition.md), every displayed endpoint product vanishes, proving symmetry on the specified domain.

To check full [self-adjointness](../../../../self-adjoint-operator.md), also identify the adjoint domain. Allow $v$ to run through the clamped domain. At either endpoint, $v''$ and $v'''$ can be chosen independently, for instance using a [polynomial](../../../../polynomial-split.md) near that endpoint multiplied by a [smooth cutoff function](../../../../smooth-cutoff-function.md). The remaining boundary form is $[\overline u v'''-\overline {u'}v'']_0^1$. It vanishes for every such $v$ precisely when $u=u'=0$ at both endpoints. These are exactly the original [boundary conditions](../../../../boundary-condition.md). On the regular finite [interval](../../../../interval-mathematics.md), the adjoint domain consequently equals $\{u\in H^4(0,1):u(0)=u'(0)=u(1)=u'(1)=0\}$, rather than a larger domain. Here $H^4$ is the [Sobolev space](../../../../sobolev-space-split.md) of [functions](../../../../function-split.md) whose [weak derivatives](../../../../weak-derivative.md) through order four are [square-integrable](../../../../square-integrable-function.md).

**The operator together with these [boundary conditions](../../../../boundary-condition.md) is fully [self-adjoint](../../../../self-adjoint-operator.md).** As a further consistency check, [integration by parts](../../../../integration-by-parts.md) gives $\langle y,Ly\rangle=\int_0^1(|y''|^2+|y|^2)\,dx>0$ for every nonzero admissible $y$. The reusable calculation is the [Lagrange identity for a fourth-order differential operator](../../../../lagrange-identity-for-a-fourth-order-differential-operator.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
