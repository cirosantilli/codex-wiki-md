<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The dimension assumption supplies a nonzero $h\in S_2(\Gamma_0(11))$. The projective index of the [Gamma 0 congruence subgroup](../../../../../../gamma-0-congruence-subgroup.md) is twelve: reduction modulo eleven identifies its cosets with the twelve points of $\mathbb P^1(\mathbb F_{11})$. There are two [modular cusps](../../../../../../cusp-of-a-modular-group.md), by the preceding classification. There are no effective elliptic fixed points. An order-two fixed point would require a root of $x^2+1$ modulo eleven, which does not exist; an order-three fixed point would require a root of $x^2+x+1$, equivalent to a nontrivial cube root of unity in a group of order ten, which also does not exist.

The [regular-cusp valence formula on a torsion-free modular curve](../../../../../../regular-cusp-valence-formula-on-a-torsion-free-modular-curve.md) therefore gives

$$
\sum_{P\in X_0(11)}\operatorname{ord}_P h=\frac{2\cdot12}{12}=2.
$$

All orders are nonnegative and both cusp orders are at least one. Thus $h$ has order exactly one at both [modular cusps](../../../../../../cusp-of-a-modular-group.md) and has no zeros in the half-plane. One way to justify the degree count here is the [genus formula for a modular curve](../../../../../../genus-formula-for-a-modular-curve.md): the same index, cusp and elliptic data give genus one. The invariant differential $h(\tau)d\tau$ has cusp order $\operatorname{ord}h-1$, because $d\tau$ is a nonzero constant times $dq_c/q_c$. Its total canonical degree $2g-2=0$ therefore makes the sum of the two cusp-adjusted orders and the interior orders zero, giving precisely the count above.

Let $H(\tau)=\Delta(\tau)\Delta(11\tau)$. By the product formula it has no zeros in the half-plane; by the cusp-order table it has order twelve at each cusp. Its weight is twenty-four. Therefore $H/h^{12}$ is a weight-zero [modular function](../../../../../../modular-function-split.md), with neither zeros nor poles anywhere on the [compactified modular curve](../../../../../../compactified-modular-curve.md). It is constant by the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) on a compact surface. Normalize $h$ so its leading [Fourier coefficient](../../../../../../fourier-coefficient.md) at infinity is one. Since $H=q^{12}+O(q^{13})$, that constant becomes one:

$$
\boxed{h^{12}=\Delta(\tau)\Delta(11\tau),\qquad
h(\tau)=q\prod_{n\geq1}(1-q^n)^2(1-q^{11n})^2.}
$$

This fixes the holomorphic twelfth root by its leading term and proves the [weight-two discriminant root at level eleven](../../../../../../weight-two-discriminant-root-at-level-eleven.md) is a nonzero member, hence a generator, of the given space. Taking an arbitrary pointwise twelfth root without this argument would not establish modularity: it could carry an unwanted character.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
