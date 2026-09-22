<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [almost complex structure](../../../../../almost-complex-manifold.md) $J$ is compatible with $\omega$ if $J^2=-I$, $\omega(Ju,Jv)=\omega(u,v)$, and $g_J(u,v)=\omega(u,Jv)$ is a positive-definite [inner product](../../../../../inner-product.md). To construct one, choose a [Riemannian metric](../../../../../riemannian-metric.md) $h$ and define $A$ by $h(Au,v)=\omega(u,v)$. The map $A$ is invertible and [skew-adjoint](../../../../../skew-adjoint-generator.md), so $-A^2$ is positive definite. Its positive square root $P=(-A^2)^{1/2}$ commutes with $A$, and

$$
J=AP^{-1},\qquad
J^2=-I,\qquad
\omega(u,Jv)=h(u,Pv)>0\quad(u=v\ne0).
$$

The same identities show that $J$ preserves $\omega$. The positive square root depends smoothly on $A$, giving a smooth [compatible almost complex structure](../../../../../compatible-almost-complex-structure.md).

For a compatible $J$, applying this [metric construction of a compatible almost complex structure](../../../../../metric-construction-of-a-compatible-almost-complex-structure.md) to $g_J$ returns $J$. Given $J_0,J_1$, apply it to $(1-t)g_{J_0}+tg_{J_1}$ to obtain a path joining them. In fact interpolation to any fixed auxiliary metric gives a contraction. Thus **the space is nonempty and connected**, and even [contractible](../../../../../contractible-space.md), by [contractibility of compatible almost complex structures](../../../../../contractibility-of-compatible-almost-complex-structures.md).

[Regularity of a J-holomorphic curve](../../../../../regularity-of-a-j-holomorphic-curve.md) $u$ means that its linearized [Cauchy–Riemann operator](../../../../../cauchy-riemann-operator.md) $D_u$ is [surjective](../../../../../surjective-function.md). Differentiating in coordinates gives

$$
D_u\xi=\partial_s\xi+J(u)\partial_t\xi
+(dJ)_u(\xi)\partial_tu,
$$

up to the harmless factor $1/2$ in the convention for $\bar\partial_J$. For constant $u$, the last term vanishes, $J(u)$ is constant, and the pulled-back tangent bundle is $\mathbb{CP}^1\times T_{u}M$. Identifying $T_uM$ with $\mathbb C^n$, this is a direct sum of $n$ copies of the [Dolbeault operator](../../../../../dolbeault-operator.md) on the trivial line bundle. Its cokernel is $H^{0,1}(\mathbb{CP}^1,\mathcal O)=0$, by [Dolbeault cohomology of the projective line](../../../../../dolbeault-cohomology-of-the-projective-line.md). Hence constant maps are regular for every compatible $J$.

The [Energy identity for a J-holomorphic curve](../../../../../energy-identity-for-a-j-holomorphic-curve.md) says that the energy is $\int_{\mathbb{CP}^1}u^*\omega$. If the [homology class](../../../../../homology-class.md) is zero, this integral is zero, forcing $du=0$. Thus **every zero-class sphere is constant and regular**.

In real dimension four, the [Fredholm index](../../../../../fredholm-index.md) of the parametrized sphere operator is $4+2c_1(A)$. At a regular nonconstant sphere, quotienting by the six-dimensional [Möbius transformation](../../../../../mobius-transformation.md) group gives a local moduli space, or an orbifold for finite stabilizers, of real dimension

$$
\boxed{2c_1(A)-2}.
$$

This is the [dimension formula for regular J-holomorphic spheres](../../../../../dimension-formula-for-regular-j-holomorphic-spheres.md).

For a [simple J-holomorphic sphere](../../../../../simple-j-holomorphic-sphere.md) in class $A$, the [adjunction inequality for a simple J-holomorphic sphere](../../../../../adjunction-inequality-for-a-simple-j-holomorphic-sphere.md) gives $c_1(A)\leq A^2+2$. If $A^2\leq-2$, the displayed moduli dimension is negative, so such a regular [simple J-holomorphic sphere](../../../../../simple-j-holomorphic-sphere.md) cannot exist. To cover nonsimple maps as well, interpret regularity here as regularity for all nonconstant maps under discussion. A degree-$m$ cover, $m\geq2$, of a [simple J-holomorphic sphere](../../../../../simple-j-holomorphic-sphere.md) in class $B$ has $A=mB$, with $B^2\leq-1$ and $c_1(B)\leq1$. Its local family of [rational covering maps of the projective line](../../../../../rational-covering-maps-of-the-projective-line.md) modulo domain reparametrization has real dimension $4m-4$, while the predicted dimension is

$$
2m\,c_1(B)-2\leq2m-2<4m-4.
$$

It therefore cannot be regular. This proves **there are no regular spheres in a class with square at most minus two**, by [negative-square exclusion under full sphere regularity](../../../../../negative-square-exclusion-under-full-sphere-regularity.md). Regularity only for simple curves would not suffice: multiple covers of an exceptional minus-one sphere are the counterexample.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
