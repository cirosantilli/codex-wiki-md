<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a locally compact space, [compactly supported cohomology](../../../../../compactly-supported-cohomology.md) is

$$
H_c^q(X;\mathbb Z)=\varinjlim_{K\subset X\text{ compact}}H^q(X,X\setminus K;\mathbb Z),
$$

with transition maps induced by enlarging supports. In $\mathbb R^n$ closed balls are cofinal; their complements retract onto $S^{n-1}$. The relative [cohomology](../../../../../cohomology-split.md) long exact sequence and contractibility of $\mathbb R^n$ give

$$
\boxed{H_c^q(\mathbb R^n;\mathbb Z)=\begin{cases}\mathbb Z,&q=n,\\0,&q\ne n.\end{cases}}
$$

This is [compactly supported cohomology of Euclidean space](../../../../../compactly-supported-cohomology-of-euclidean-space.md); for $n=0$ it is simply the [cohomology](../../../../../cohomology-split.md) of a point.

For an oriented $n$-manifold without boundary, [Poincare duality](../../../../../poincare-duality.md) in its compact-support form states that capping with the locally finite [fundamental class](../../../../../fundamental-class.md) gives $H_c^q(M;\mathbb Z)\cong H_{n-q}(M;\mathbb Z)$. If $M$ is closed, the ordinary [fundamental class](../../../../../fundamental-class.md) $[M]\in H_n(M;\mathbb Z)$ gives $H^q(M;\mathbb Z)\cong H_{n-q}(M;\mathbb Z)$ and a perfect complementary-degree pairing over $\mathbb Q$.

Choose an oriented embedded closed ball $B$ in a connected closed oriented $M$. Collapse $M\setminus\operatorname{int}B$ to a point, identifying $B/\partial B$ with $S^n$ using its orientation. The quotient map is continuous. By [excision](../../../../../excision-theorem.md), the [fundamental class](../../../../../fundamental-class.md) maps to the local oriented generator in $H_n(B,\partial B)$, and then to the generator of $H_n(S^n)$. Hence **the collapse map has $\boxed{\deg f=1}$**.

The reverse direction is not always possible. More generally a degree-one map $f:N\to M$ between closed oriented manifolds induces an injective map on rational [cohomology](../../../../../cohomology-split.md): if $\alpha\ne0$, duality supplies $\beta$ with $\langle\alpha\smile\beta,[M]\rangle\ne0$, and

$$
\langle f^*\alpha\smile f^*\beta,[N]\rangle
=\deg(f)\langle\alpha\smile\beta,[M]\rangle\ne0.
$$

In particular **there is no degree-one map $S^2\to T^2$**, since $H^1(T^2;\mathbb Q)=\mathbb Q^2$ but $H^1(S^2;\mathbb Q)=0$. This is a counterexample to an unconditional reverse assertion.

Finally let $p:\mathbb{CP}^3\to S^4$ be the given bundle projection. The standard [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md) is $H^*(\mathbb{CP}^3;\mathbb Z)=\mathbb Z[h]/(h^4)$, $|h|=2$; the integral generator $u$ of $H^4(S^4)$ has $p^*u=mh^2$ for some integer $m$. If a [section of a fiber bundle](../../../../../section-fiber-bundle.md) $s$ existed, $p\circ s=1$ would give $s^*p^*=1$ by functoriality. But $H^2(S^4)=0$, so $s^*h=0$ and $s^*(mh^2)=0$, contradicting $s^*p^*u=u\ne0$. The facts used here are the sphere [cohomology](../../../../../cohomology-split.md) groups, the projective-space ring just stated, and multiplicative functoriality of [cohomology](../../../../../cohomology-split.md). Thus **the bundle has no section**, the [cohomological obstruction to a section of the twistor bundle](../../../../../cohomological-obstruction-to-a-section-of-the-twistor-bundle.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
