<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work in the [prime end](../../../../../prime-end.md) [closure](../../../../../closure-topology.md) of the marked domain, so that its two conformal [boundary](../../../../../boundary-of-a-set.md) points are distinct even if their physical [boundary](../../../../../boundary-of-a-set.md) representatives coincide. A [chordal filling](../../../../../chordal-filling.md) is a closed connected set joining those points, meeting the conformal [boundary](../../../../../boundary-of-a-set.md) nowhere else, and full relative to the two [boundary](../../../../../boundary-of-a-set.md) arcs between them: complementary pockets that do not reach either [boundary](../../../../../boundary-of-a-set.md) arc have been added. In the normalized [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), its two complementary sides are [simply connected](../../../../../simply-connected-space.md) and abut the negative and positive real axes. For a proper boundary-to-boundary curve, [chordal filling](../../../../../chordal-filling.md) means adjoining all such trapped pockets to its range. Independent curves are combined by taking their union and then applying this same [chordal filling](../../../../../chordal-filling.md) operation.

An admissible marked subdomain $V\subset U$ contains neighborhoods of the two marked [boundary](../../../../../boundary-of-a-set.md) points and has a [simply connected](../../../../../simply-connected-space.md) component joining them. The restriction property says that, conditional on the random [chordal filling](../../../../../chordal-filling.md) $K$ being contained in $V$, its law is the [chordal filling](../../../../../chordal-filling.md) law for $(V,z_0,z_1)$. Equivalently, mapping the conditional [chordal filling](../../../../../chordal-filling.md) conformally back to $(U,z_0,z_1)$ recovers the original law. The contained-set events are understood away from the shared marked endpoints.

By transporting the family under [conformal maps](../../../../../conformal-map.md), it suffices to work in $(\mathbb H,0,\infty)$. Let $A$ be an admissible [compact H-hull](../../../../../compact-h-hull.md) whose [closure](../../../../../closure-topology.md) avoids zero, and normalize

$$
\Phi_A:\mathbb H\setminus A\longrightarrow\mathbb H,
\qquad\Phi_A(0)=0,\quad\Phi_A'(\infty)=1.
$$

In terms of the single normalized measure $\mu$, restriction is precisely

$$
\boxed{\mathcal L(\Phi_A(K)\mid K\cap A=\varnothing)=\mu.}
$$

The [Schwarz reflection principle](../../../../../schwarz-reflection-principle.md) extends $\Phi_A$ analytically near zero, with $\Phi_A'(0)>0$, so the stated conditioning events have positive probability for the two laws considered below. This is the [chordal restriction property](../../../../../chordal-restriction-property.md) for filled sets. An unbounded marked subdomain can be approximated by such compact-hull removals; [conformal maps](../../../../../conformal-map.md) transport the formulation to general domains.

We need a determination principle for filled sets, since a probability of one avoidance event alone would not establish equality of laws. Choose countably many thin polygonal [compact H-hulls](../../../../../compact-h-hull.md) with rational data, attached to real [boundary](../../../../../boundary-of-a-set.md) intervals away from zero. For each [chordal filling](../../../../../chordal-filling.md), every point of its complement has a path within one of the two complementary sides to the appropriate real [boundary](../../../../../boundary-of-a-set.md) interval. A sufficiently thin tube along such a path avoids the [chordal filling](../../../../../chordal-filling.md) and contains a neighborhood of that point. Hence the union of interiors of all avoided test tubes is exactly the complement.

Their joint avoidance probabilities are also determined by single-hull probabilities. For a finite union of test [compact H-hulls](../../../../../compact-h-hull.md), either the union separates zero from infinity, in which case a connected [chordal filling](../../../../../chordal-filling.md) cannot avoid it, or its unbounded complementary component contains both marked endpoints. In the latter case fill the union's bounded pockets to get an admissible [compact H-hull](../../../../../compact-h-hull.md) $C$. A connected set joining zero to infinity and avoiding the union cannot enter one of these separated pockets, so it avoids $C$ as well. Thus joint avoidance is either impossible or is the avoidance event for $C$. The [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) gives every finite joint [probability distribution](../../../../../probability-distribution.md) of the tube-avoidance indicators, and these indicators determine the random complement and [chordal filling](../../../../../chordal-filling.md). This proves [avoidance probabilities determine a chordal filling law](../../../../../avoidance-probabilities-determine-a-chordal-filling-law.md).

In the given avoidance formulas, the argument of the conformal map must be the retained open domain, rather than the random closed filling. We express that domain as $\mathbb H\setminus A$ to keep the two objects distinct. The formulas then imply for the two filled processes

$$
p_\gamma(A)=\Phi_A'(0)^{5/8},\qquad p_E(A)=\Phi_A'(0).
$$

The [chordal filling](../../../../../chordal-filling.md) operation does not change avoidance of an admissible [compact H-hull](../../../../../compact-h-hull.md): every piece of that [compact H-hull](../../../../../compact-h-hull.md) is attached to the real [boundary](../../../../../boundary-of-a-set.md) away from the endpoints, and so cannot be inside a trapped pocket while its generating curve avoids the [compact H-hull](../../../../../compact-h-hull.md). These laws are conformally invariant as unparameterized [chordal filling](../../../../../chordal-filling.md) laws. For [SLE](../../../../../schramm-loewner-evolution.md) this follows from Question 1; for the [Brownian half-plane excursion](../../../../../brownian-excursion-in-the-upper-half-plane.md), [Brownian scaling](../../../../../brownian-scaling.md) of its independent one- and three-dimensional coordinates shows that its unparameterized law is unchanged by positive dilations, and mapping the [Brownian half-plane excursion](../../../../../brownian-excursion-in-the-upper-half-plane.md) to another marked domain gives the conformally natural law. [Conformal invariance of planar Brownian motion](../../../../../conformal-invariance-of-planar-brownian-motion.md) describes the corresponding change of time, which does not alter the [chordal filling](../../../../../chordal-filling.md).

Here is the conditional-law calculation for either exponent $\alpha\in\{5/8,1\}$. For another admissible [compact H-hull](../../../../../compact-h-hull.md) $B$ in the image [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), set

$$
C=A\cup\Phi_A^{-1}(B),\qquad\Phi_C=\Phi_B\circ\Phi_A.
$$

The complement of $C$ is mapped to $\mathbb H$ by this composition, so $C$ is again admissible; both maps fix zero and have [derivative](../../../../../derivative.md) one at infinity. The chain rule gives $\Phi_C'(0)=\Phi_B'(0)\Phi_A'(0)$. Therefore

$$
\begin{aligned}
\mathbb P(\Phi_A(K)\cap B=\varnothing\mid K\cap A=\varnothing)
&=\frac{\mathbb P(K\cap C=\varnothing)}{\mathbb P(K\cap A=\varnothing)}\\
&=\frac{\Phi_C'(0)^\alpha}{\Phi_A'(0)^\alpha}
=\Phi_B'(0)^\alpha.
\end{aligned}
$$

These are exactly the original [chordal filling](../../../../../chordal-filling.md)'s avoidance probabilities for every $B$. The determination principle proves equality of the conditional image law with the original law. Hence **both generated [chordal fillings](../../../../../chordal-filling.md) have restriction**, with exponents $5/8$ and $1$ respectively. This is a complete implication from the two allowed avoidance formulas; the restriction conclusion was not assumed.

For independent [chordal fillings](../../../../../chordal-filling.md), avoidance of $A$ by their filled union is equivalent to avoidance by every component. [Independence](../../../../../independent-random-variables.md) multiplies the probabilities, and thus adds their [restriction exponents of a chordal filling](../../../../../restriction-exponent-of-a-chordal-filling.md). Consequently

$$
\mathbb P(\overline\gamma^{\otimes8}\cap A=\varnothing)
=\bigl(\Phi_A'(0)^{5/8}\bigr)^8
=\Phi_A'(0)^5
=\bigl(\Phi_A'(0)\bigr)^5
=\mathbb P(\overline E^{\otimes5}\cap A=\varnothing).
$$

The determination principle applies once more, giving

$$
\boxed{\mathcal L(\overline\gamma^{\otimes8})=\mathcal L(\overline E^{\otimes5}).}
$$

The equality concerns the filled, unparameterized closed sets. The numerical reason is $8\cdot(5/8)=5\cdot1=5$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
