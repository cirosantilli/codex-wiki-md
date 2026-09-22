<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work over $\mathbb Q$ and put $b_i=\dim H^i(M;\mathbb Q)$. For a closed [orientable](../../../../../orientable-surface.md) six-dimensional [manifold](../../../../../topological-manifold.md), [Poincare duality](../../../../../poincare-duality.md) gives $b_i=b_{6-i}$, so

$$
\chi(M)=2(b_0-b_1+b_2)-b_3.
$$

The remaining [Betti number](../../../../../betti-number.md) is even. Indeed, the [cup product](../../../../../cup-product.md) pairing

$$
H^3(M;\mathbb Q)\times H^3(M;\mathbb Q)\longrightarrow\mathbb Q,
\qquad (u,v)\longmapsto\langle u\smile v,[M]\rangle
$$

is nondegenerate by duality and skew-symmetric by graded commutativity, since $(-1)^{3\cdot3}=-1$. If its dimension were odd, a matrix $A$ for it would satisfy $\det A=\det(-A^T)=-\det A$, forcing $\det A=0$ in characteristic zero, a contradiction. Thus $b_3$ is even and

$$
\boxed{\chi(M)\equiv0\pmod2.}
$$

This is the [Euler characteristic parity in dimensions congruent to two modulo four](../../../../../euler-characteristic-parity-in-dimensions-congruent-to-two-modulo-four.md). If the [manifold](../../../../../topological-manifold.md) has several components, apply the argument to each component and add.

The orientability assumption is essential. The [Real projective space](../../../../../real-projective-space.md) $\mathbb {RP}^6$ has one cell in each dimension from zero to six, giving

$$
\chi(\mathbb {RP}^6)=1-1+1-1+1-1+1=\boxed{1}.
$$

It is nonorientable: its double cover $S^6$ has the [orientation](../../../../../orientation-of-a-simplex.md)-reversing antipodal deck transformation, of degree $(-1)^7=-1$.

For the construction, $\mathbb {CP}^3$ is a closed [orientable](../../../../../orientable-surface.md) real six-dimensional [manifold](../../../../../topological-manifold.md) with cells in dimensions $0,2,4,6$, hence [Euler characteristic](../../../../../euler-characteristic.md) four. The product $S^3\times S^3$ is also closed and [orientable](../../../../../orientable-surface.md), with [Euler characteristic](../../../../../euler-characteristic.md) $\chi(S^3)^2=0$. The six-sphere has [Euler characteristic](../../../../../euler-characteristic.md) two.

In dimension six, removing an open ball subtracts one from the [Euler characteristic](../../../../../euler-characteristic.md). To see this, write $M$ as the punctured [manifold](../../../../../topological-manifold.md) joined to a closed ball along $S^5$, whose [Euler characteristic](../../../../../euler-characteristic.md) is zero, and apply the cellular inclusion-exclusion formula. Gluing two punctured manifolds along $S^5$ therefore gives

$$
\chi(M\mathbin{\#}N)=\chi(M)+\chi(N)-2.
$$

A [connected sum](../../../../../connected-sum-of-oriented-manifolds.md) of $r$ copies of $\mathbb {CP}^3$ and $s$ copies of $S^3\times S^3$ has

$$
\chi=2+2r-2s,
$$

with the empty sum interpreted as $S^6$. Given any even integer $n$, take

$$
r=\max\{n/2-1,0\},\qquad
s=\max\{1-n/2,0\}.
$$

Both are nonnegative integers and the displayed [Euler characteristic](../../../../../euler-characteristic.md) equals $n$. Hence **[every even integer is the Euler characteristic of a closed oriented six-manifold](../../../../../every-even-integer-is-the-euler-characteristic-of-a-closed-oriented-six-manifold.md)**, including zero and negative integers; the construction is connected.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
