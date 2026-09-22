# p-adic integer

↑ **Parent:** [P-adic valuation](p-adic-valuation.md)

The [p-adic integers](p-adic-integer.md) retain arithmetic information modulo arbitrarily high powers of one [prime number](prime-number-split.md) $p$. They form the [subring](subring.md)

$$
\boxed{\mathbb Z_p=\{x\in\mathbb Q_p:|x|_p\leq1\}}
$$

of the [P-adic numbers](p-adic-number.md). Their [p-adic absolute value](p-adic-absolute-value.md) bounds the allowed denominators: **$1/3$ belongs to $\mathbb Z_2$, while $1/2$ does not**. The name therefore describes a local arithmetic [ring](ring.md), not just the ordinary [integers](integer-split.md).[§3, printed pp. 6–7: definition of Zp, rational denominators and units](p-adic-numbers-by-jan-hendrik-evertse.md)

A concrete description gives an element by a compatible [sequence](sequence.md) of [congruence classes](congruence-class.md):

$$
\mathbb Z_p=\varprojlim_{n\geq1}\mathbb Z/p^n\mathbb Z,\qquad
r_{n+1}\equiv r_n\pmod{p^n}.
$$

The [inverse limit](inverse-limit.md) condition says that gaining more precision must preserve the digits already determined. Each $r_n$ is a residue modulo $p^n$; choosing its least nonnegative [integer](integer-split.md) representative gives $0\leq r_n<p^n$. The ordinary integer $13$ gives residues $1,1,5,13$ modulo $2,4,8,16$.

<a id="image-compatible-binary-residues-describe-successive-finite-precisions-of-a-2-adic-integer"></a>
![](padic-compatible-binary-residue-tree.png)

**[Figure 13](#image-compatible-binary-residues-describe-successive-finite-precisions-of-a-2-adic-integer). Compatible binary residues describe successive finite precisions of a 2-adic integer**. Original full residue tree through modulus $16$. Each edge reduces a residue to its parent modulus; the highlighted path follows the integer $13$. Four binary digits determine the entire [coset](coset.md) $13+16\mathbb Z_2$, leaving infinitely many higher-digit choices. Choosing all later digits zero selects the ordinary integer $13$.

The useful feature is that one exact object organizes an unlimited family of finite [modular arithmetic](modular-arithmetic-split.md) calculations. [Addition](addition.md) and [multiplication](multiplication.md) are performed modulo each $p^n$, and the results remain compatible. A [p-adic digit](p-adic-digit.md) expansion makes this concrete:

$$
x=\sum_{j\geq0}b_jp^j,\qquad b_j\in\{0,1,\ldots,p-1\},\qquad
r_n=\sum_{j=0}^{n-1}b_jp^j.
$$

The expansion is unique and converges in the [p-adic metric](p-adic-metric.md); its higher powers have smaller [p-adic absolute value](p-adic-absolute-value.md). The [digit agreement and p-adic distance](digit-agreement-and-p-adic-distance.md) criterion tells exactly which finite digits a precision bound preserves.[§3, Theorem 3.4 and digit/congruence discussion, printed pp. 7–9: unique expansion and agreement of low-order digits](p-adic-numbers-by-jan-hendrik-evertse.md)

**Table of contents**

- [p-adic digit](p-adic-digit.md)
  - [Digit agreement and p-adic distance](digit-agreement-and-p-adic-distance.md)
- [Modular inversion converges to a p-adic inverse](modular-inversion-converges-to-a-p-adic-inverse.md)
- [Ring structure of the p-adic integers](ring-structure-of-the-p-adic-integers.md)
- [Open subgroups of the p-adic integers](open-subgroups-of-the-p-adic-integers.md)
- [7-adic integer](7-adic-integer.md)
- [2-adic integer](2-adic-integer.md)
- [Topological generator of the additive group of p-adic integers](topological-generator-of-the-additive-group-of-p-adic-integers.md)

## ↑ Ancestors (5)

1. [P-adic valuation](p-adic-valuation.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (41)

- [2-adic integer](2-adic-integer.md)
- [7-adic integer](7-adic-integer.md)
- [Binomial polynomial](binomial-polynomial.md)
- [Coleman norm-fixed lift](coleman-norm-fixed-lift.md)
- [Continuous functions on the p-adic integers](continuous-functions-on-the-p-adic-integers.md)
- [Cyclic finite quotients of the p-adic augmentation filtration](cyclic-finite-quotients-of-the-p-adic-augmentation-filtration.md)
- [Digit agreement and p-adic distance](digit-agreement-and-p-adic-distance.md)
- [Discrete antidifferentiation on the p-adic integers](discrete-antidifferentiation-on-the-p-adic-integers.md)
- [Mahler coefficient exponential generating function](mahler-coefficient-exponential-generating-function.md)
- [Mahler expansion of continuous p-adic functions](mahler-expansion-of-continuous-p-adic-functions.md)
- [Open subgroups of the p-adic integers](open-subgroups-of-the-p-adic-integers.md)
- [p-adic digit](p-adic-digit.md)
- [p-adic integer](p-adic-integer.md)
- [p-adic metric](p-adic-metric.md)
- [P-adic number](p-adic-number.md)
- [P-adic unit](p-adic-unit.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-24/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-85/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-28/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-29/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-26/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-27/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-136/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-136/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-151/2/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-101/2/a/solution.md)
- [Powerful Lie algebra over p-adic integers](powerful-lie-algebra-over-p-adic-integers.md)
- [Powerful pro-p group](powerful-pro-p-group.md)
- [Procyclic group](procyclic-group.md)
- [Profinite abelian group](profinite-abelian-group.md)
- [Ring structure of the p-adic integers](ring-structure-of-the-p-adic-integers.md)
- [Strong completeness of finitely generated pro-p groups](strong-completeness-of-finitely-generated-pro-p-groups.md)
- [Tate module](tate-module.md)
- [Translation-invariant linear forms on p-adic continuous functions vanish](translation-invariant-linear-forms-on-p-adic-continuous-functions-vanish.md)
- [Ultrametric space](ultrametric-space.md)
- [Uniform group and powerful Lie lattice correspondence](uniform-group-and-powerful-lie-lattice-correspondence.md)
- [Uniform pro-p group](uniform-pro-p-group.md)
- [Uniform pro-p group and powerful Lie lattice correspondence](uniform-pro-p-group-and-powerful-lie-lattice-correspondence.md)
- [Zp-extension](zp-extension.md)
