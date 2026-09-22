<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [covariant quantization of the bosonic string](../../../../../../covariant-quantization-of-the-bosonic-string.md),

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_j^m,\alpha_k^n]=j\eta^{mn}\delta_{j+k,0},\qquad
(\alpha_k^m)^\dagger=\alpha_{-k}^m.
$$

All other commutators between independent [canonical variables](../../../../../../canonical-variables.md) vanish. The covariant [Fock vacuum](../../../../../../fock-vacuum.md) obeys $\alpha_k^m|0;p\rangle=0$ for every $k>0$ and every $m$. [Normal ordering](../../../../../../normal-ordering.md) moves these annihilating [string oscillators](../../../../../../string-oscillator.md) to the right and gives

$$
\widehat L_j=\frac12\sum_{k\in\mathbb Z}:\alpha_{j-k}\cdot\alpha_k:,
\qquad
\widehat L_0=\frac{p^2}{2\pi T}+\widehat N_{\mathrm{cov}},\qquad
\widehat N_{\mathrm{cov}}=\sum_{k>0}\alpha_{-k}\cdot\alpha_k.
$$

Then $\widehat N_{\mathrm{cov}}|0;p\rangle=0$. Its commutator $[\widehat N_{\mathrm{cov}},\alpha_{-k}^m]=k\alpha_{-k}^m$ grades a [Fock state](../../../../../../fock-state.md) basis by $N=\sum k n_{km}$, although its [inner product](../../../../../../inner-product.md) is indefinite because of the timelike oscillator.

The quantum [Virasoro algebra](../../../../../../virasoro-algebra.md) has [central charge](../../../../../../central-charge.md) $D$:

$$
\boxed{[\widehat L_j,\widehat L_k]=(j-k)\widehat L_{j+k}
+\frac D{12}j(j^2-1)\delta_{j+k,0}.}
$$

The [Virasoro central extension](../../../../../../virasoro-central-extension.md) comes from [commutators](../../../../../../commutator.md) needed to order infinite oscillator sums; it is a quantum effect absent from the classical [Poisson brackets](../../../../../../poisson-bracket.md). Replacing a classical [Poisson bracket](../../../../../../poisson-bracket.md) by a [commutator](../../../../../../commutator.md) cannot recover that term without a regularized ordering calculation.

If a state were annihilated by every nonzero $\widehat L_j$, the $j=1,k=-1$ [commutator](../../../../../../commutator.md) would imply $\widehat L_0|\psi\rangle=0$. The $j=2,k=-2$ commutator would then imply $(D/2)|\psi\rangle=0$. For $D>0$, **only the zero vector is annihilated by all nonzero [Virasoro constraints](../../../../../../virasoro-constraint.md)**. This explains why only positive modes annihilate a [physical string state](../../../../../../physical-string-state.md).

The vacuum is a [physical string state](../../../../../../physical-string-state.md) when $p^2=2\pi Ta$. At level one all states have the form $|A;p\rangle=A_m\alpha_{-1}^m|0;p\rangle$. Since $[\widehat L_j,\alpha_k^m]=-k\alpha_{j+k}^m$, the positive-mode [Virasoro constraints](../../../../../../virasoro-constraint.md) give

$$
\widehat L_1|A;p\rangle=\frac{A\cdot p}{\sqrt{\pi T}}|0;p\rangle,\qquad
\widehat L_j|A;p\rangle=0\quad(j\geq2).
$$

Thus the complete level-one conditions and norm are

$$
\boxed{p^2=2\pi T(a-1),\qquad A\cdot p=0,\qquad
\langle A;p|A;p\rangle=A_m^*\eta^{mn}A_n,}
$$

with the common vacuum normalization suppressed.

For $a>1$, choose spacelike [momentum](../../../../../../momentum.md) $p^m=(0,k,0,\ldots)$, $k^2=2\pi T(a-1)$. A purely timelike polarization has $A\cdot p=0$ and norm $-1$. Hence **a negative-norm [physical string state](../../../../../../physical-string-state.md) exists when $a>1$**.

For $a<1$, the [mass-shell condition](../../../../../../string-mass-shell-condition.md) gives $M^2=2\pi T(1-a)>0$. In a rest frame, $A\cdot p=0$ forces $A_0=0$, leaving $D-1$ positive-norm [vector-particle polarizations](../../../../../../vector-particle-polarization.md), those of a massive vector.

For $a=1$ and nonzero null [momentum](../../../../../../momentum.md), $A\cdot p=0$ leaves a null direction $A_m\propto p_m$. The corresponding [null string state](../../../../../../null-string-state.md) is $p\cdot\alpha_{-1}|0;p\rangle=\sqrt{\pi T}\widehat L_{-1}|0;p\rangle$. It is orthogonal to every [physical string state](../../../../../../physical-string-state.md) because $\widehat L_1$ annihilates them. Quotienting by this [gauge redundancy](../../../../../../gauge-redundancy.md), $A_m\sim A_m+\zeta p_m$, leaves $D-2$ positive [vector-particle polarizations](../../../../../../vector-particle-polarization.md). Thus **the level-one spectrum agrees with [light-cone gauge in string theory](../../../../../../light-cone-gauge-in-string-theory.md) at $a=1$**. This level-one argument alone does not establish consistency or absence of negative norms at all higher levels.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
