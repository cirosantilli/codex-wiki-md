<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The dense commutant orbit makes $\Omega$ separating for $M$, so $S_0(a\Omega)=a^*\Omega$ is well defined on the dense subspace $M\Omega$. Put $\tau(a)=\langle a\Omega,\Omega\rangle$. The assumed identity says that this positive [vector](../../../../../../vector.md) functional is a [tracial positive functional](../../../../../../tracial-positive-functional.md). Hence

$$
\|S_0(a\Omega)\|^2=\tau(aa^*)=\tau(a^*a)=\|a\Omega\|^2.
$$

It extends to an antiunitary involution $J$ on $H$, with $J\Omega=\Omega$. This is the [modular conjugation](../../../../../../modular-conjugation.md), and the [modular operator](../../../../../../modular-operator.md) in this tracial case is $\Delta=I$.

On the dense subspace $M\Omega$,

$$
(JaJ)(b\Omega)=J(ab^*\Omega)=ba^*\Omega.
$$

Thus it acts by right multiplication and commutes with all left multiplications; $JMJ\subseteq M'$. We prove the reverse inclusion rather than assuming the general Tomita commutation theorem.

Let $T\in M'$, $C=\|T\|$, and $\eta=T\Omega$. The set

$$
\mathcal B=\{a\Omega:a\in M,\ \|a\|\leq C\}
$$

is [weakly compact](../../../../../../weakly-compact-set.md) and convex. Indeed, [trace-class duality](../../../../../../trace-class-duality.md) and the [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) make the bounded-operator ball compact in a topology stronger than the [weak operator topology](../../../../../../weak-operator-topology.md). The algebra $M$ is weak-operator closed, and $a\mapsto a\Omega$ is weakly continuous, so its image is [weakly compact](../../../../../../weakly-compact-set.md).

For $b\in M$ use the [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) $b=uh$, $h=|b|$. Both $h$ and $u$ belong to $M$: [continuous functional calculus](../../../../../../continuous-functional-calculus.md) gives $h$, and $b(h+\varepsilon I)^{-1}$ tends strongly to $u$. The polar decomposition is proved independently in Question 8. Since $T$ commutes with $M$,

$$
\langle T\Omega,b\Omega\rangle
=\langle T h^{1/2}u^*\Omega,h^{1/2}\Omega\rangle.
$$

The [trace](../../../../../../matrix-trace.md) identity gives

$$
\|h^{1/2}u^*\Omega\|^2=\tau(uhu^*)=\tau(hu^*u)=\tau(h),
\qquad \|h^{1/2}\Omega\|^2=\tau(h).
$$

Therefore $|\langle\eta,b\Omega\rangle|\leq C\tau(h)$. Meanwhile

$$
\sup_{a\in M,\ \|a\|\leq C}\operatorname{Re}\langle a\Omega,b\Omega\rangle
=C\tau(h),
$$

with the supremum attained by $a=Cu$. For the upper bound, traciality gives $\tau(b^*a)=\tau(h^{1/2}u^*a h^{1/2})$; evaluating this on $\Omega$ bounds its absolute value by $\|a\|\tau(h)$.

These support inequalities imply $\eta\in\mathcal B$. Otherwise the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) would separate $\eta$ from this closed [convex set](../../../../../../convex-set.md) by a real inner-product functional. Since $M\Omega$ is dense, its separating [vector](../../../../../../vector.md) could be approximated by some $b\Omega$, preserving strict separation, contrary to the displayed inequality. Thus $T\Omega=a\Omega$ for an $a\in M$ of [norm](../../../../../../norm.md) at most $C$.

The [bounded operator](../../../../../../continuous-linear-operator.md) $R_a=Ja^*J$ commutes with $M$ and sends $\Omega$ to $a\Omega$. It agrees with $T$ on the cyclic [vector](../../../../../../vector.md) and therefore on all of $M\Omega$, hence on $H$. This proves $T\in JMJ$, and so

$$
\boxed{JMJ=M'.}
$$

For the regular representation, take $\Omega=\delta_e$. It is cyclic for the left action and for the commuting right action. On finite sums of left translations, its [vector](../../../../../../vector.md) functional is the identity coefficient, so $\tau(ab)=\tau(ba)$. This extends to the whole [group von Neumann algebra](../../../../../../group-von-neumann-algebra.md) by the bounded strong-star approximations of Question 6, taking limits of the [vector](../../../../../../vector.md) functional and products. The conjugation is explicitly

$$
(J\xi)(h)=\overline{\xi(h^{-1})},\qquad J\lambda(g)J=\rho(g).
$$

Consequently

$$
\boxed{\lambda(\Gamma)'=J\lambda(\Gamma)''J=\rho(\Gamma)''.}
$$

Thus the commutant in (b) is exactly the [Von Neumann algebra](../../../../../../von-neumann-algebra.md) of right regular translations, with the inverse in $\rho(g)$ fixing the representation convention.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
