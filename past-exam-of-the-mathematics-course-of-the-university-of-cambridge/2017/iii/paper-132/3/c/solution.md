<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the closed [genus](../../../../../../genus-of-a-surface.md) $g\geq2$ version of [Teichmüller's uniqueness theorem](../../../../../../teichmuller-s-uniqueness-theorem.md). Let $f_0:X\to Y$ be a [Teichmüller map](../../../../../../teichmuller-map.md): for a nonzero [holomorphic quadratic differential](../../../../../../holomorphic-quadratic-differential.md) $q$, normalized by $\int_X|q|=1$, and $0<k_0<1$,

$$
\mu_{f_0}=k_0\frac{|q|}{q},\qquad K_0=\frac{1+k_0}{1-k_0}.
$$

The value at a zero of $q$ is irrelevant to the [Beltrami coefficient](../../../../../../beltrami-coefficient.md), which is defined almost everywhere. For every [quasiconformal map](../../../../../../quasiconformal-mapping.md) $f:X\to Y$ preserving [orientation](../../../../../../orientation-of-a-simplex.md) and [homotopic](../../../../../../homotopy.md) to $f_0$, the conclusion is

$$
\boxed{K(f)\geq K_0,\qquad K(f)=K_0\ \Longrightarrow\ f=f_0.}
$$

The normalized $q$ is also uniquely determined when $k_0>0$.

We use the following analytic input, stated with its hypotheses. The [Reich–Strebel inequality](../../../../../../reich-strebel-inequality.md) says that if $f_0$ has the displayed [Beltrami coefficient](../../../../../../beltrami-coefficient.md) and a competitor $f$ has the same target and [homotopy class](../../../../../../homotopy-class.md), then, for $\mu=\mu_f$,

$$
K_0\leq\int_X\frac{|1+\mu q/|q||^2}{1-|\mu|^2}\,|q|.
$$

This is the standard fundamental inequality for an integrable [holomorphic quadratic differential](../../../../../../holomorphic-quadratic-differential.md); it also holds on a finite-type punctured surface with the homotopy fixing the punctures. Its formulation is given in [Gardiner and Hu, §5](https://userhome.brooklyn.cuny.edu/gardiner/A%20short%20course%20on%20Teichmuller%27s%20theorem.pdf). We quote this analytic inequality as the lecture result used in the proof.

Put $k=\|\mu\|_\infty$. Pointwise, away from the isolated zeros of $q$,

$$
\frac{|1+\mu q/|q||^2}{1-|\mu|^2}
\leq\frac{(1+|\mu|)^2}{1-|\mu|^2}
=\frac{1+|\mu|}{1-|\mu|}
\leq\frac{1+k}{1-k}.
$$

Integrating against the [probability density function](../../../../../../probability-density-function.md) $|q|$ proves $K_0\leq K(f)$. If $K(f)=K_0$, all these inequalities are equalities almost everywhere. The strictly increasing last function forces $|\mu|=k_0$ almost everywhere; equality in the [triangle inequality](../../../../../../triangle-inequality.md) then forces $\mu q/|q|=k_0$. Therefore

$$
\mu_f=\mu_{f_0}\quad\text{almost everywhere}.
$$

Two [quasiconformal maps](../../../../../../quasiconformal-mapping.md) with the same [Beltrami coefficient](../../../../../../beltrami-coefficient.md) differ by postcomposition with a [biholomorphism](../../../../../../biholomorphism.md), by the local chain rule for the [Beltrami equation](../../../../../../beltrami-equation.md). Consequently $h=f\circ f_0^{-1}$ is a [biholomorphism](../../../../../../biholomorphism.md) from $Y$ to itself [homotopic](../../../../../../homotopy.md) to the identity.

For completeness, such a [biholomorphism](../../../../../../biholomorphism.md) is the identity when $g\geq2$. Apply the [uniformization theorem](../../../../../../uniformization-theorem.md) and choose the lift of the homotopy to $\mathbb H$ starting at the identity. Its endpoint lift $\widetilde h$ commutes with every [deck transformation](../../../../../../deck-transformation.md). It is a real [Möbius transformation](../../../../../../mobius-transformation.md). The [compact](../../../../../../compact-space.md) quotient has no [parabolic Möbius transformations](../../../../../../parabolic-element-of-psl2-r.md) in its deck group, and freeness excludes [elliptic Möbius transformations](../../../../../../elliptic-element-of-psl2-r.md). Two distinct hyperbolic axes exist: a discrete free group preserving just one axis would be cyclic, contradicting the [fundamental group](../../../../../../fundamental-group.md) of a [closed surface](../../../../../../closed-surface.md) of [genus](../../../../../../genus-of-a-surface.md) at least two. Commutation with two [deck transformations](../../../../../../deck-transformation.md) represented by [hyperbolic Möbius transformations](../../../../../../hyperbolic-element-of-psl2-r.md) having distinct axes makes it fix their boundary endpoints individually; there are at least three such endpoints. A [Möbius transformation](../../../../../../mobius-transformation.md) fixing three points is the identity. Hence $h=\operatorname{id}$ and $f=f_0$.

If $q_1$ is another unit-area differential for the same map, then $|q_1|/q_1=|q|/q$, so $q_1/q$ is positive real wherever defined. This [meromorphic function](../../../../../../meromorphic-function.md) is constant by the [open mapping theorem](../../../../../../open-mapping-theorem-functional-analysis.md), and normalization makes the constant one. Without normalization, positive multiples of $q$ describe the same map. At $k_0=0$, uniqueness of the map still holds in [genus](../../../../../../genus-of-a-surface.md) at least two, but there is no distinguished $q$. In [genus](../../../../../../genus-of-a-surface.md) one, translations supply nontrivial [biholomorphisms](../../../../../../biholomorphism.md) [homotopic](../../../../../../homotopy.md) to the identity, so equality determines the map only up to those [biholomorphisms](../../../../../../biholomorphism.md); the [genus](../../../../../../genus-of-a-surface.md) hypothesis cannot be omitted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
