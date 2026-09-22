<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a bounded connected domain with the [interior cone property](../../../../../../interior-cone-property.md), and $1\leq p<n$, the mean-zero form of the [Poincaré inequality](../../../../../../poincare-inequality.md) is

$$
\boxed{\|v-v_\Omega\|_{L^p(\Omega)}\leq C_{\Omega,p}\|\nabla v\|_{L^p(\Omega)},\qquad v_\Omega=\frac1{|\Omega|}\int_\Omega v.}
$$

No zero boundary trace is imposed. Subtracting the mean is essential because nonzero constants have zero [gradient](../../../../../../gradient.md).

Suppose the estimate failed. Subtract means and normalize to obtain $v_j\in W^{1,p}(\Omega)$ with

$$
\int_\Omega v_j=0,\qquad\|v_j\|_p=1,\qquad\|\nabla v_j\|_p\longrightarrow0.
$$

This sequence is bounded in the [Sobolev space](../../../../../../sobolev-space-split.md) $W^{1,p}$. The allowed [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md) on cone domains provides a subsequence converging strongly in $L^p(\Omega)$ to $v$. Its mean is zero and its [norm](../../../../../../norm.md) is one. For any compactly supported smooth [test function](../../../../../../test-function.md) $\phi$,

$$
\int v\partial_i\phi=\lim_j\int v_j\partial_i\phi=-\lim_j\int(\partial_i v_j)\phi=0.
$$

Thus every [weak derivative](../../../../../../weak-derivative.md) of $v$ vanishes. To show this implies constancy, mollify on any ball compactly contained in $\Omega$. The resulting smooth function has zero [gradient](../../../../../../gradient.md) and is constant on the smaller ball. Passing to its $L^p$ limit makes $v$ constant almost everywhere on that ball. Overlapping balls have the same constant, and [connectedness](../../../../../../connected-space.md) connects any two points by a chain of such balls. Hence $v$ is constant almost everywhere throughout $\Omega$. Its zero mean makes it zero, contradicting [norm](../../../../../../norm.md) one. This proves the stated [Poincaré inequality](../../../../../../poincare-inequality.md). The frequently used stronger Sobolev-Poincare formulation also follows: with $p^*=np/(n-p)$, the cone-domain [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) gives $\|w\|_{p^*}\leq C_S(\|w\|_p+\|\nabla w\|_p)$. Insert $w=v-v_\Omega$ and the estimate just proved to obtain

$$
\boxed{\|v-v_\Omega\|_{L^{p^*}(\Omega)}\leq C_S(1+C_{\Omega,p})\|\nabla v\|_{L^p(\Omega)}.}
$$

Thus both the same-exponent and critical-exponent mean-zero versions are covered. Connectedness cannot be dropped without subtracting a separate mean on every component. The usual meaning of the stated range is $1\leq p<n$; $W^{1,p}$ with $p<1$ is not part of this Sobolev-space formulation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
