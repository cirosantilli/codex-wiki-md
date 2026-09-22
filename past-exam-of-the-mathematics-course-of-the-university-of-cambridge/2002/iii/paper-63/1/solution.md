<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $|m,m'\rangle$ as shorthand for the [tensor product](../../../../../tensor-product.md) of two total-[isospin](../../../../../isospin.md)-one states with third components $m,m'$. A total-[isospin](../../../../../isospin.md)-zero state must have total third component zero, so write $a|1,-1\rangle+b|0,0\rangle+c|-1,1\rangle$. Applying the total [raising operator](../../../../../raising-operator.md) gives

$$
I_+\bigl(a|1,-1\rangle+b|0,0\rangle+c|-1,1\rangle\bigr)
=\sqrt2\bigl[(a+b)|1,0\rangle+(b+c)|0,1\rangle\bigr].
$$

An [isospin](../../../../../isospin.md) singlet must be annihilated by this operator; hence $b=-a$ and $c=a$. Normalization gives the [two-isovector singlet](../../../../../two-isovector-singlet.md)

$$
\boxed{|I=0,M=0\rangle=\frac{|1,-1\rangle-|0,0\rangle+|-1,1\rangle}{\sqrt3}.}
$$

It is also annihilated by the total [lowering operator](../../../../../lowering-operator.md). A raising or lowering action changes the third-component label by one; the unchanged output label in the PDF's preliminary ladder formula is a typographical omission, not the action used here.

Exchange commutes with the total [isospin](../../../../../isospin.md) operators. The displayed singlet is symmetric. The $I=2$ multiplet has symmetric highest state $|1,1\rangle$; applying the symmetric total [lowering operator](../../../../../lowering-operator.md) preserves that exchange symmetry. The symmetric square of a three-dimensional space has dimension six, exactly $1+5$, while its antisymmetric square has dimension three. The remaining $I=1$ multiplet is therefore antisymmetric. Thus the [Clebsch-Gordan decomposition](../../../../../clebsch-gordan-decomposition.md) is

$$
\mathbf3\otimes\mathbf3=\mathbf1_S\oplus\mathbf3_A\oplus\mathbf5_S.
$$

[Pions](../../../../../pion.md) have zero intrinsic [spin](../../../../../spin.md) and form an [isospin](../../../../../isospin.md) triplet. [Bose-Einstein statistics](../../../../../bose-einstein-statistics.md) requires the complete two-pion state to be symmetric under exchange. Its relative orbital state changes by $(-1)^\ell$, so odd [orbital angular momentum](../../../../../orbital-angular-momentum.md) requires antisymmetric [isospin](../../../../../isospin.md): **an odd-$\ell$ two-pion state has $I=1$**. This statement treats the charge components as states of the same [isospin](../../../../../isospin.md) multiplet, rather than ignoring exchange when their charges differ.

For the decay, let $|\chi\rangle=H_I|K^0\rangle$. The stated commutator with $I_3$ gives $I_3|\chi\rangle=0$. More decisively, the commuting [raising operator](../../../../../raising-operator.md) gives

$$
I_+^2|\chi\rangle=H_I I_+^2|K^0\rangle=0.
$$

The kaon doublet cannot be raised twice. An $I=2,M=0$ component would survive two raisings, so it is excluded. Meanwhile a spinless [kaon](../../../../../kaon.md) decaying into two spinless [pions](../../../../../pion.md) has $\ell=0$ by conservation of total [angular momentum](../../../../../angular-momentum.md), independently of whether parity is conserved by the decay. The exchange condition excludes $I=1$. This proves the [highest-weight weak-isospin selection in kaon decay](../../../../../highest-weight-weak-isospin-selection-in-kaon-decay.md): **the two-pion final state has $I=0$**.

In a consistent pion phase convention, the singlet's charge components have the structure

$$
|0,0\rangle=\frac{|\pi^+\pi^-\rangle+|\pi^-\pi^+\rangle-|\pi^0\pi^0\rangle}{\sqrt3}.
$$

The normalized symmetric charged channel has coefficient $\sqrt{2/3}$ and the neutral channel coefficient $-1/\sqrt3$. Thus, in the [isospin](../../../../../isospin.md) limit with equal pion masses and matching two-body phase space,

$$
\boxed{\frac{\Gamma(K^0\to\pi^+\pi^-)}{\Gamma(K^0\to\pi^0\pi^0)}=2.}
$$

Equivalently, ordered charged and neutral amplitudes have equal magnitudes, but neutral identical particles contribute the phase-space factor $1/2!$. This is the same counting expressed in another basis, and must not be included a second time after using the normalized charge-channel coefficients. Small pion-mass and electromagnetic effects can modify the ideal ratio.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
