<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [almost complex structure](../../../../../almost-complex-manifold.md) is a smooth endomorphism $J:TM\to TM$ with $J^2=-I$; in particular the real dimension is even. Complexifying the [tangent bundle](../../../../../tangent-bundle.md) splits it into the $i$ and $-i$ eigensubbundles

$$
T_{\mathbb C}M=T^{1,0}M\oplus T^{0,1}M,
$$

interchanged by conjugation. On a [complex manifold](../../../../../complex-manifold.md), these are locally spanned by $\partial_{z^j}$ and $\partial_{\bar z^j}$. An [integrable almost complex structure](../../../../../integrable-almost-complex-structure.md) is one arising from a holomorphic coordinate atlas. Its $T^{0,1}$ sections are closed under the [Lie bracket](../../../../../lie-bracket.md). The obstruction is the [Nijenhuis tensor](../../../../../nijenhuis-tensor.md)

$$
N_J(X,Y)=[JX,JY]-J[JX,Y]-J[X,JY]-[X,Y].
$$

Expanding this expression in the two eigentypes shows that $N_J=0$ is equivalent to involutivity of $T^{0,1}$. Holomorphic coordinates make this condition necessary; the [Newlander-Nirenberg theorem](../../../../../newlander-nirenberg-theorem.md) gives its sufficiency for smooth $J$. Integrability also gives $d=\partial+\bar\partial$, with $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$. The [Dolbeault operator](../../../../../dolbeault-operator.md) on $T^{1,0}M=T'_M$ defines its [holomorphic vector bundle](../../../../../holomorphic-vector-bundle.md) structure.

A real [connection on a vector bundle](../../../../../connection-vector-bundle.md) $\nabla$ on $TM$ preserves $J$ when $\nabla J=0$. Its complexification then preserves both eigensubbundles. Restricting to $T'_M$ gives a complex connection $D$. Conversely any complex connection on $T'_M$ gives such a real connection by adjoining its conjugate on $T^{0,1}$ and restricting to the conjugation-fixed real tangent bundle. Equivalently, transfer $D$ through the real isomorphism $v\mapsto(v-iJv)/2$. These operations are inverse. **Preserving $J$ alone does not impose the holomorphic compatibility condition $D^{0,1}=\bar\partial_{T'}$.**

For integrable $J$, the latter condition has a precise real-connection interpretation: the mixed-type [torsion tensor](../../../../../torsion-tensor.md) vanishes. In holomorphic coordinates it says $D_{\partial_{\bar z^i}}\partial_{z^j}=0$. Reality also gives $\nabla_{\partial_{z^j}}\partial_{\bar z^i}=0$. Since these coordinate fields commute, their torsion is zero. Conversely a $J$-preserving real connection with zero mixed torsion has these two derivatives equal; they belong to opposite eigentypes, so both vanish, proving $D^{0,1}=\bar\partial_{T'}$. This is the [holomorphic tangent connection and mixed torsion criterion](../../../../../holomorphic-tangent-connection-and-mixed-torsion-criterion.md).

Full torsion-freeness imposes the additional symmetry $\Gamma^k_{ij}=\Gamma^k_{ji}$ in $D_{\partial_{z^i}}\partial_{z^j}=\Gamma^k_{ij}\partial_{z^k}$, and its conjugate. Such a $J$-preserving torsion-free connection exists on any [complex manifold](../../../../../complex-manifold.md): local holomorphic-coordinate flat connections have these properties, and a real [partition of unity](../../../../../partition-of-unity.md) combines them globally. Preservation of $J$ and zero torsion persist because both conditions are affine in the connection. Conversely if $J$ is merely almost complex, a torsion-free connection preserving it forces $N_J=0$: replace brackets by $\nabla_XY-\nabla_YX$ in the displayed tensor and use $\nabla J=0$; all terms cancel. Thus this connection condition detects integrability, without imposing any metric condition.

A [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) is a real [Riemannian metric](../../../../../riemannian-metric.md) $g$ with $g(JX,JY)=g(X,Y)$. It induces a Hermitian metric $h$ on $T'_M$ and the fundamental two-form $\omega(X,Y)=g(JX,Y)$. The unique [Chern connection](../../../../../chern-connection.md) satisfies both $D^{0,1}=\bar\partial_{T'}$ and metric compatibility. In a holomorphic frame with metric matrix $H$ and coefficient-column convention, its matrix is $H^{-1}\partial H$. It need not be torsion-free when transferred to $TM$.

In holomorphic coordinates its coefficients are $\Gamma^k_{ij}=h^{k\bar l}\partial_i h_{j\bar l}$. Their symmetry in $i,j$ is equivalent to $\partial_i h_{j\bar l}=\partial_j h_{i\bar l}$, which says $\partial\omega=0$. The conjugate gives $\bar\partial\omega=0$. The result that a [torsion-free Chern tangent connection characterizes a Kähler metric](../../../../../torsion-free-chern-tangent-connection-characterizes-a-kahler-metric.md) follows: **the transferred Chern connection is torsion-free exactly when $\boxed{d\omega=0}$**, the [Kähler metric](../../../../../kahler-metric.md) condition. In that case it equals the [Levi-Civita connection](../../../../../levi-civita-connection.md), by uniqueness of the metric-compatible torsion-free connection. Equivalently a Hermitian metric is Kähler exactly when its [Levi-Civita connection](../../../../../levi-civita-connection.md) preserves $J$. In the reverse direction $\nabla J=0$ implies $\nabla\omega=0$, and zero torsion gives $d\omega=0$.

This explains the role of [Kähler metrics](../../../../../kahler-metric.md): they make the real Riemannian and holomorphic connection theories coincide. A general [complex manifold](../../../../../complex-manifold.md) has torsion-free $J$-preserving connections and has Hermitian metrics, but need not have a connection satisfying both requirements simultaneously. On a [Kähler manifold](../../../../../kahler-manifold.md), the [Kähler identities](../../../../../kahler-identities.md) then link the [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) and [Hodge Laplacian](../../../../../hodge-laplacian.md), giving $\Delta_d=2\Delta_{\bar\partial}=2\Delta_\partial$ and the resulting harmonic [Hodge decomposition theorem for compact Kähler manifolds](../../../../../hodge-decomposition-theorem-for-compact-kahler-manifolds.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
