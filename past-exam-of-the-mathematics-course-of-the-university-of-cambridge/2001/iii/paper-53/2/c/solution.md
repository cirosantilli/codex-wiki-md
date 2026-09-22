<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work in a normalized [analytic function](../../../../../../space-of-holomorphic-functions.md) space of even [unimodal maps](../../../../../../unimodal-interval-map.md) with a quadratic critical maximum. The relevant fixed-point and spectral conjectures are that the [period-doubling renormalization operator](../../../../../../period-doubling-renormalization-operator.md) has a nontrivial universal [Feigenbaum renormalization fixed point](../../../../../../feigenbaum-renormalization-fixed-point.md) $g$, and that its [linearization](../../../../../../linearization.md) at $g$ is hyperbolic with precisely one expanding [eigenvalue](../../../../../../eigenvalue.md) $\delta>1$. Its remaining spectral directions contract. The associated local [stable manifold](../../../../../../stable-manifold.md) has [finite codimension](../../../../../../finite-codimension-in-a-banach-space.md) one; maps on it are indefinitely renormalizable and their normalized central return maps converge to $g$. The local [unstable manifold](../../../../../../unstable-manifold.md) has dimension one and organizes the basic period-doubling and superstable transitions. These assertions concern the normalized quadratic universality class, rather than arbitrary functions or every parameter family.

The [hyperbolicity mechanism for period-doubling universality](../../../../../../hyperbolicity-mechanism-for-period-doubling-universality.md) explains parameter scaling. Let a typical one-parameter family cross the [stable manifold](../../../../../../stable-manifold.md) transversely at $\mu=s_\infty$. In local stable and unstable coordinates, write its unstable coordinate as

$$
u(\mu)=c(\mu-s_\infty)+O((\mu-s_\infty)^2),\qquad c\ne0.
$$

Repeated renormalization multiplies this coordinate to leading order by $\delta$ while damping stable components. A superstable orbit of period $2^n$ becomes a superstable two-cycle after $n-1$ renormalizations. Hence its parameter is characterized by arrival at the same basic superstable surface, at a fixed nonzero unstable coordinate after the initial transient. This yields

$$
s_\infty-s_n=C\delta^{-n}(1+o(1)),\qquad C>0,
$$

and therefore

$$
\boxed{\frac{s_n-s_{n-1}}{s_{n+1}-s_n}\longrightarrow\delta.}
$$

The family-dependent coefficient $C$ changes with parametrization, but the ratio does not. The same argument applies to the primary bifurcation surfaces and their successive preimages. [Transversality](../../../../../../transversality-of-a-map-to-a-submanifold.md) matters: a family tangent to the [stable manifold](../../../../../../stable-manifold.md) need not display this generic parameter exponent.

Spatial universality follows from the [fixed point](../../../../../../fixed-point.md)'s scale $a_g=g(1)<0$. As renormalized maps approach $g$, their successive central restrictive intervals shrink by factors approaching $|a_g|$, with orientation alternating. Thus the signed central spacings have asymptotic ratio $a_g^{-1}$, and

$$
\boxed{\alpha=-a_g^{-1}.}
$$

Stable directions remove the original family's detailed shape; the limiting profile is $g$, the parameter expansion rate is $\delta$, and the spatial contraction rate is $|a_g|$. Families with the same quadratic critical order therefore share the same [Feigenbaum constants](../../../../../../feigenbaum-constants.md). A different even critical order gives a different [Feigenbaum fixed point](../../../../../../feigenbaum-renormalization-fixed-point.md) and a different universality class. This explanation is a consequence of the fixed-point, hyperbolicity and transverse-transition properties; it is not a proof that an arbitrary one-parameter family satisfies those properties.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
