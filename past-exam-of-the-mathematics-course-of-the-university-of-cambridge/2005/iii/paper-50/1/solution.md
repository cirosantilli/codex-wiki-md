<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a finite-dimensional [unitary representation](../../../../../unitary-representation.md) of [SU(2)](../../../../../su-2-group.md) and units $\hbar=1$, so the [isospin](../../../../../isospin.md) generators are [Hermitian](../../../../../hermitian-operator.md) and $I_+^\dagger=I_-$. Their commutators are

$$
[I_3,I_\pm]=\pm I_\pm,\qquad[I_+,I_-]=2I_3.
$$

On the normalized [highest-weight vector](../../../../../highest-weight-vector.md), the given [quadratic Casimir operator](../../../../../quadratic-casimir-operator.md) identity gives $\mathbf I^2|I,I\rangle=I(I+1)|I,I\rangle$. Since the [quadratic Casimir operator](../../../../../quadratic-casimir-operator.md) commutes with every generator, this eigenvalue is unchanged down the ladder. Each application of $I_-$ lowers $M$ by one. For a normalized descendant,

$$
\|I_-|I,M\rangle\|^2=\langle I,M|I_+I_-|I,M\rangle=I(I+1)-M^2+M=(I+M)(I-M+1).
$$

Positivity first gives $I\ge0$. In a finite-dimensional representation the descending ladder must terminate; the norm vanishes only at $M=-I$. Thus the number of lowering steps is $2I$, a nonnegative integer, and

$$
\boxed{I\in\{0,\tfrac12,1,\tfrac32,\ldots\},\qquad I_-^{2I+1}|I,I\rangle=0.}
$$

For $M>-I$, define the normalized descendant by dividing $I_-|I,M\rangle$ by its positive norm. This fixes its relative phase and gives

$$
I_-|I,M\rangle=\sqrt{(I+M)(I-M+1)}|I,M-1\rangle.
$$

Acting with $I_+$ and using $I_+I_-=\mathbf I^2-I_3^2+I_3$ proves

$$
I_+|I,M-1\rangle=\sqrt{(I+M)(I-M+1)}|I,M\rangle.
$$

The resulting [isospin multiplet](../../../../../isospin-multiplet.md) has $2I+1$ states. More explicitly,

$$
|I,M\rangle=\sqrt{\frac{(I+M)!}{(2I)!(I-M)!}}\,I_-^{I-M}|I,I\rangle.
$$

The factorial arguments are integers, even for half-integer $I$.

Put $R(\theta)=e^{-i\theta I_2}$. Differentiation and the commutators give

$$
R(\theta)I_1R(\theta)^{-1}=I_1\cos\theta-I_3\sin\theta,\qquad R(\theta)I_3R(\theta)^{-1}=I_3\cos\theta+I_1\sin\theta,
$$

while $I_2$ is unchanged. Hence at the half-turn,

$$
\boxed{RI_1R^{-1}=-I_1,\quad RI_2R^{-1}=I_2,\quad RI_3R^{-1}=-I_3,\qquad R=e^{-i\pi I_2}.}
$$

The half-turn preserves $I$ and reverses $M$, so $R|I,M\rangle=\alpha_M|I,-M\rangle$. Since $RI_+R^{-1}=-I_-$, comparison of the two ways to rotate a raised state gives $\alpha_{M+1}=-\alpha_M$.

To fix the remaining phase, expand the supplied highest-state rotation identity as a finite sum. The $k$th term is

$$
\frac{(\cos(\theta/2))^{2I-k}(\sin(\theta/2))^k}{k!}I_-^k|I,I\rangle,\qquad0\le k\le2I.
$$

As $\theta\uparrow\pi$, all terms vanish except $k=2I$. The product of the lowering coefficients gives $I_-^{2I}|I,I\rangle=(2I)!|I,-I\rangle$. The surviving coefficient is therefore one, fixing $\alpha_I=1$. The [half-turn phase of an SU(2) multiplet](../../../../../half-turn-phase-of-an-su-2-multiplet.md) is

$$
\boxed{\alpha_M=(-1)^{I-M}.}
$$

In particular the recurrence and highest-state phase are consistent with $R^2=(-1)^{2I}$.

[Charge conjugation](../../../../../charge-conjugation.md) is a linear unitary symmetry. If $J_i=CI_iC^{-1}$, conjugation preserves the commutator and the scalar $i$, so

$$
[J_i,J_j]=C[I_i,I_j]C^{-1}=i\epsilon_{ijk}J_k.
$$

Thus the conjugated generators obey the same [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md). The [charge conjugation](../../../../../charge-conjugation.md) action on $(I_1,I_2,I_3)$ is exactly the same pair of sign reversals as $R$. Their product $G=CR$ consequently satisfies $GI_iG^{-1}=I_i$ for all $i$. For integer $I$, its value on the neutral member is

$$
G|I,0\rangle=(-1)^I C|I,0\rangle=\eta(-1)^I|I,0\rangle.
$$

Commuting $G$ through the [ladder operators](../../../../../ladder-operator.md) transfers that value to every state in the same [isospin multiplet](../../../../../isospin-multiplet.md). Therefore the [G-parity of an isospin multiplet](../../../../../g-parity-of-an-isospin-multiplet.md) is

$$
\boxed{G|I,M\rangle=\eta(-1)^I|I,M\rangle.}
$$

A [photon](../../../../../photon.md) has [charge conjugation](../../../../../charge-conjugation.md) value minus one, so a two-photon state has value plus one. The electromagnetic two-photon decay preserves [charge conjugation](../../../../../charge-conjugation.md), giving $\eta_{\pi^0}=+1$. Since the [pion](../../../../../pion.md) has $I=1$, all three [pion](../../../../../pion.md) charge states have [G parity](../../../../../g-parity.md) minus one:

$$
\boxed{G|\pi^{+,0,-}\rangle=-|\pi^{+,0,-}\rangle.}
$$

The [rho meson](../../../../../rho-meson.md) has $I=1$, $\eta=-1$, hence $G_\rho=+1$, whereas the [omega meson](../../../../../omega-meson.md) has $I=0$, $\eta=-1$, hence $G_\omega=-1$. On an $n$-pion state the internal symmetry acts on each [pion](../../../../../pion.md), giving $(-1)^n$ independently of orbital [angular momentum](../../../../../angular-momentum.md). Conservation of [G parity](../../../../../g-parity.md) in the isospin-symmetric [strong interaction](../../../../../strong-interaction.md) therefore gives the [G-parity selection rule for pion multiplicities](../../../../../g-parity-selection-rule-for-pion-multiplicities.md):

$$
\boxed{\rho\to2\pi\text{ allowed},\quad\omega\to3\pi\text{ allowed},\quad\rho\not\to3\pi,\quad\omega\not\to2\pi.}
$$

The allowed channels can also satisfy [angular momentum](../../../../../angular-momentum.md) and physical parity: the two [pions](../../../../../pion.md) from a rho can have relative orbital [angular momentum](../../../../../angular-momentum.md) one and total [isospin](../../../../../isospin.md) one, while three [pions](../../../../../pion.md) can couple to the omega's $I=0$, $J^P=1^-$. The rule refers to the ideal isospin-conserving strong amplitude; small symmetry-breaking or electromagnetic contributions are not excluded.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
