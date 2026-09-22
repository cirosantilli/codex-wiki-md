<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

[Sunada's theorem](../../../../../sunada-theorem.md) states that if a [finite group](../../../../../finite-group.md) $T$ acts isometrically on a closed [Riemannian manifold](../../../../../riemannian-manifold.md) $X$, and two [Gassmann equivalent](../../../../../gassmann-equivalence.md) [subgroups](../../../../../subgroup.md) $H_1,H_2$ act freely, then $H_1\backslash X$ and $H_2\backslash X$ are isospectral for the function [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md). [Gassmann equivalence](../../../../../gassmann-equivalence.md) means $|H_1\cap C|=|H_2\cap C|$ for every [conjugacy class](../../../../../conjugacy-class.md) $C$ of $T$. For each [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) [eigenspace](../../../../../eigenspace.md) $E_\lambda$, its [invariant subspace](../../../../../invariant-subspace.md) has [dimension](../../../../../dimension-vector-space.md)

$$
\dim E_\lambda^{H_i}=\frac1{|H_i|}\sum_{h\in H_i}\operatorname{tr}(h|E_\lambda).
$$

The [character of a representation](../../../../../character-of-a-representation.md) is a [class function](../../../../../class-function.md), so the two [multiplicities](../../../../../multiplicity-mathematics.md) agree. A necessary condition for nonisometry is that the [subgroups](../../../../../subgroup.md) are not conjugate in $T$: conjugation by an ambient deck transformation would induce an [isometry](../../../../../isometry.md). This is not sufficient when the common covering has additional geometric symmetries.

Use the oriented [hyperbolic triangle group](../../../../../hyperbolic-triangle-group.md)

$$
\Gamma=\langle a,b:a^3=b^3=(ab)^6=1\rangle
$$

and the epimorphism $\rho:\Gamma\to T$ given by $a\mapsto s$, $b\mapsto d$. Its base [orbifold](../../../../../orbifold.md) is the doubled hyperbolic triangle with angles $\pi/3,\pi/3,\pi/6$, having signature $(0;3,3,6)$. Let $K=\ker\rho$ and $K_i=\rho^{-1}(H_i)$.

The groups $K_i$ are torsion free. Indeed, [torsion elements](../../../../../torsion-element.md) in an oriented triangle [group](../../../../../group-split.md) are conjugate to nontrivial powers of its three vertex rotations. Such powers map either to elements of order three, which cannot lie in a [subgroup](../../../../../subgroup.md) of order $96/12=8$, or to the order-two cube $z=(sd)^3$. The latter is central and absent from both $H_i$, so it is absent from every conjugate as well. Thus the degree-twelve [orbifold](../../../../../orbifold.md) covers

$$
N_i=K_i\backslash\mathbb H^2
$$

are smooth, closed, connected [orientable](../../../../../orientable-surface.md) surfaces. The common cover $X=K\backslash\mathbb H^2$ is smooth too; $H_i$ act freely on it. [Orbifold](../../../../../orbifold.md) [Euler characteristic](../../../../../euler-characteristic.md) gives

$$
\boxed{\chi(N_i)=12\left(\frac13+\frac13+\frac16-1\right)=-2,\qquad\operatorname{genus}(N_i)=2.}
$$

For example, this formula follows by triangulating the base and weighting a vertex of order $r$ by $1/r$ before multiplying by the cover degree. Equivalently, each doubled triangle has hyperbolic area $\pi/3$, so $N_i$ has area $4\pi$ and [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives the same [genus](../../../../../genus-of-a-surface.md).

There is one extra issue in obtaining the same hyperbolic limit on a single marked surface: the two limiting hyperbolic covers must themselves be isometric. Nonconjugacy and the displayed element orders alone do not prove this. An explicit realization of the supplied example resolves the issue. The [group](../../../../../group-split.md) seed is recorded in [the original genus-two construction](https://arxiv.org/pdf/math/0512519); the following coset actions and reflection identities give a direct verification. Label the twelve sheets so that the two right-coset actions of $s,d$ are

$$
\begin{aligned}
s_1&=(1\ 3\ 6)(2\ 11\ 7)(4\ 8\ 9)(5\ 10\ 12),\\
d_1&=(1\ 12\ 8)(2\ 3\ 7)(4\ 5\ 10)(6\ 9\ 11),\\
s_2&=(1\ 6\ 12)(2\ 8\ 11)(3\ 7\ 10)(4\ 5\ 9),\\
d_2&=(1\ 6\ 10)(2\ 8\ 9)(3\ 5\ 11)(4\ 7\ 12).
\end{aligned}
$$

These are concrete permutation data for an order-$96$ realization with the required two [subgroups](../../../../../subgroup.md). The permutation

$$
P=(1\ 3\ 10\ 2)(4\ 9)(5\ 8)(6\ 7)(11\ 12)
$$

satisfies, by direct substitution,

$$
Ps_1=s_2^{-1}P,\qquad Pd_1=d_2^{-1}P.
$$

Reflection of the doubled triangle reverses both vertex rotations. Apply this reflection on every [fundamental domain](../../../../../fundamental-domain.md) and relabel sheets by $P$. The two identities ensure that identified edges go to identified edges, so this descends to a hyperbolic [isometry](../../../../../isometry.md) $F_0:N_1\to N_2$. Fix $N=N_1$, let $g$ be its [hyperbolic metric](../../../../../hyperbolic-metric.md), and use $F_0$ to mark $N_2$ by the same smooth surface. Thus both pulled-back limiting [Riemannian metrics](../../../../../riemannian-metric.md) are exactly $g$. The explicit reversed-action check is what makes the common limit justified, rather than treating it as a consequence of [Sunada's theorem](../../../../../sunada-theorem.md).

Choose smooth [orbifold](../../../../../orbifold.md) [Riemannian metrics](../../../../../riemannian-metric.md) $h_k$ on the base converging to its [hyperbolic metric](../../../../../hyperbolic-metric.md) $h_0$, with no nonidentity [local isometry](../../../../../local-isometry.md) on the regular part. The density assertion in [Sunada's local isometry lemma](../../../../../sunada-local-isometry-lemma.md) applies in [orbifold](../../../../../orbifold.md) charts as well: use equivariant perturbations at the finitely many cone points and ordinary local perturbations elsewhere. Smoothness here is [orbifold](../../../../../orbifold.md) smoothness, so the lifted [Riemannian metrics](../../../../../riemannian-metric.md) on $X$ and the two smooth covers are ordinary smooth [Riemannian metrics](../../../../../riemannian-metric.md). Such choices can be made in successively smaller smooth neighbourhoods of $h_0$; cone orders and the topological coverings stay fixed.

For [area separation of convergent Sunada families](../../../../../area-separation-of-convergent-sunada-families.md), adjust each $h_k$ by a constant positive factor so that

$$
\operatorname{area}(h_k)=\operatorname{area}(h_0)(1+2^{-k}).
$$

Explicitly, multiply the initially chosen [Riemannian metric](../../../../../riemannian-metric.md) by the ratio of the desired area to its actual area. In [dimension](../../../../../dimension-vector-space.md) two this ratio is exactly the area multiplier. The ratios tend to one, so smooth convergence persists, and constant scaling preserves the absence of [local isometries](../../../../../local-isometry.md). Lift these adjusted [Riemannian metrics](../../../../../riemannian-metric.md) to $N_i$ and pull them back by the fixed markings to obtain $g_{ik}$, for $i=1,2$. The three required properties follow below.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
