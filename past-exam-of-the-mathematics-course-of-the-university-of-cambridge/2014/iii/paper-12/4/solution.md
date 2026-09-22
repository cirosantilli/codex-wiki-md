<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a closed oriented $d$-dimensional [manifold](../../../../../topological-manifold.md) $M$ and a commutative coefficient ring $R$, [Poincare duality](../../../../../poincare-duality.md) says that [cap product](../../../../../cap-product.md) with the [fundamental class](../../../../../fundamental-class.md) is an isomorphism

$$
\boxed{-\frown[M]:H^q(M;R)\overset{\cong}{\longrightarrow}H_{d-q}(M;R).}
$$

Over a field it equivalently gives a nondegenerate [Poincare duality pairing](../../../../../poincare-duality-pairing.md) $(a,b)\mapsto\langle a\smile b,[M]\rangle$ between complementary cohomological degrees.

For the six-manifold take rational coefficients and write $b_j=\dim_{\mathbb Q}H^j(X;\mathbb Q)$. [Poincare duality](../../../../../poincare-duality.md) gives $b_j=b_{6-j}$, so the [Euler characteristic](../../../../../euler-characteristic.md) is

$$
\chi(X)=2(b_0-b_1+b_2)-b_3.
$$

The middle-degree [Poincare duality pairing](../../../../../poincare-duality-pairing.md) on $H^3(X;\mathbb Q)$ is skew-symmetric by [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md), since $(-1)^{3\cdot3}=-1$. It is a nondegenerate [alternating bilinear form](../../../../../alternating-bilinear-form.md), so its dimension $b_3$ is even. For example, a nonsingular skew-symmetric matrix of odd size would have $\det A=\det(-A)=-\det A$, impossible over $\mathbb Q$. Therefore **$\boxed{\chi(X)\in2\mathbb Z}$.**

To realize every even integer, use $\chi(S^6)=2$, $\chi(\mathbb{CP}^3)=4$ and $\chi(S^3\times S^3)=0$. All three are closed connected orientable six-manifolds. For the [connected sum of oriented manifolds](../../../../../connected-sum-of-oriented-manifolds.md), removing a ball from each summand and gluing their boundary spheres gives

$$
\chi(M\#N)=\chi(M)+\chi(N)-2
$$

in dimension six: each removed open ball decreases the Euler characteristic by one, while the gluing sphere $S^5$ has Euler characteristic zero. If $k=2\ell$, put

$$
r=\max(\ell-1,0),\qquad s=\max(1-\ell,0),\qquad X_k=S^6\#\bigl(\#^r\mathbb{CP}^3\bigr)\#\bigl(\#^s(S^3\times S^3)\bigr),
$$

omitting zero copies. The [Euler characteristic](../../../../../euler-characteristic.md) is $2+2r-2s=k$. This supplies **a closed connected orientable example for every $k\in2\mathbb Z$**.

Without orientability, evenness need not hold. The [Real projective space](../../../../../real-projective-space.md) $\mathbb{RP}^6$ is a closed six-manifold with one cell in each dimension $0,\ldots,6$, so

$$
\boxed{\chi(\mathbb{RP}^6)=1.}
$$

It is nonorientable because the antipodal deck transformation on $S^6$ has degree $(-1)^7=-1$ and reverses orientation. Thus it gives the required counterexample.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
