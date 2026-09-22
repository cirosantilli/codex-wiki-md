<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use Euclidean coordinates $(x^1,x^2,x^3,x^4)$ and orientation $dx^1\wedge dx^2\wedge dx^3\wedge dx^4$. For $D_\mu=\partial_\mu+A_\mu$, the [gauge curvature](../../../../../gauge-field-strength.md) is $F_{\mu\nu}=[D_\mu,D_\nu]$. The [ASDYM equations](../../../../../anti-self-dual-yang-mills-equations.md) are $F=-*F$, equivalently

$$
F_{12}+F_{34}=0,\qquad F_{13}-F_{24}=0,\qquad F_{14}+F_{23}=0.
$$

Put $w=x^1+ix^2$, $z=x^3+ix^4$, with $\partial_w=(\partial_1-i\partial_2)/2$ and similarly for $z$. The bars label the complex conjugate coordinates on the Euclidean real slice; after complexification they can be treated as independent coordinates. A [Lax pair for the anti-self-dual Yang-Mills equations](../../../../../lax-pair-for-the-anti-self-dual-yang-mills-equations.md) is

$$
\boxed{(D_w-\lambda D_{\bar z})\Psi=0,\qquad
(D_z+\lambda D_{\bar w})\Psi=0,\qquad \lambda\in\mathbb{CP}^1.}
$$

At infinity rescale the operators and use the other affine coordinate. Their [commutator](../../../../../commutator.md) is

$$
[D_w-\lambda D_{\bar z},D_z+\lambda D_{\bar w}]
=F_{wz}+\lambda(F_{w\bar w}+F_{z\bar z})+\lambda^2F_{\bar w\bar z}.
$$

Compatibility for every $\lambda$ is therefore precisely $F_{wz}=F_{\bar w\bar z}=0$ and $F_{w\bar w}+F_{z\bar z}=0$. To verify the real component signs,

$$
F_{wz}=\frac14\{F_{13}-F_{24}-i(F_{14}+F_{23})\},\qquad
F_{w\bar w}+F_{z\bar z}=\frac i2(F_{12}+F_{34}).
$$

The conjugate equation supplies the remaining real components. This is compatibility of an overdetermined system, not an additional field equation on $\Psi$ for only one value of the [spectral parameter](../../../../../spectral-parameter.md).

Impose invariance under translations in $x^1,x^2,x^3$, writing $t=x^4$. In a symmetry-adapted gauge the potentials depend only on $t$. A further $t$-dependent [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) sets $A_4=0$ locally, by solving the usual [parallel transport](../../../../../parallel-transport.md) ordinary differential equation; it does not reintroduce spatial dependence. Then

$$
F_{ab}=[A_a,A_b],\qquad F_{a4}=-\dot A_a.
$$

The three real equations above become $\dot A_1=[A_2,A_3]$, $\dot A_2=[A_3,A_1]$ and $\dot A_3=[A_1,A_2]$, namely

$$
\boxed{\dot A_a=\frac12\epsilon_{abc}[A_b,A_c].}
$$

These are the [Nahm equations](../../../../../nahm-equations.md). The orientation chosen above gives the requested plus sign; reversing orientation exchanges [self-duality of gauge curvature](../../../../../self-duality-of-gauge-curvature.md) and [anti-self-duality of gauge curvature](../../../../../anti-self-duality-of-gauge-curvature.md). Translation invariance here is a local dimensional reduction and is not a claim of finite four-dimensional action over all three translation directions.

To prove conservation, abbreviate $P=A_1+iA_2$, $Q=A_1-iA_2$ and $R=A_3$, so $A(\lambda)=P+2R\lambda-Q\lambda^2$ and $B(\lambda)=-iR+iQ\lambda$. Expanding the [commutator](../../../../../commutator.md), including the cancellation of the cubic term, gives

$$
[A(\lambda),B(\lambda)]
=-i[P,R]+i[P,Q]\lambda+i[R,Q]\lambda^2.
$$

The [Nahm equations](../../../../../nahm-equations.md) give

$$
\dot P=-i[P,R],\qquad
2\dot R=i[P,Q],\qquad
-\dot Q=i[R,Q].
$$

Thus the [polynomial Lax representation of the Nahm equations](../../../../../polynomial-lax-representation-of-the-nahm-equations.md) is

$$
\boxed{\dot A(\lambda)=[A(\lambda),B(\lambda)].}
$$

Take a finite-dimensional [matrix](../../../../../matrix.md) representation of the [Lie algebra](../../../../../lie-algebra-split.md) and its complexification. For every positive integer $p$, differentiating the product and using cyclicity of the [matrix trace](../../../../../matrix-trace.md) gives

$$
\frac d{dt}\operatorname{Tr}(A(\lambda)^p)
=p\operatorname{Tr}(A(\lambda)^{p-1}[A(\lambda),B(\lambda)])
=p\{\operatorname{Tr}(A^pB)-\operatorname{Tr}(BA^p)\}=0.
$$

This proves the [trace invariants of a Lax equation](../../../../../trace-invariants-of-a-lax-equation.md) directly. Since $\operatorname{Tr}(A(\lambda)^p)$ is a polynomial of degree at most $2p$ in the affine coordinate $\lambda$, its derivative vanishes identically only if the derivative of every coefficient vanishes. Therefore **every trace-polynomial coefficient is independent of $t$**. At projective infinity these polynomials are sections of $\mathcal O(2p)$; they need not be constant functions of $\lambda$ on the whole projective [sphere](../../../../../sphere.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
