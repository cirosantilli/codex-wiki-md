# Entropy of mixing

↑ **Parent:** [Ideal solution](ideal-solution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_of_mixing)

The entropy of mixing is the [entropy](entropy-split.md) change between initially separate components and their final [mixture](mixture-split.md), with initial and final [temperatures](temperature-split.md), [pressures](pressure-split.md) and component [amount of substance](amount-of-substance.md) values specified. For an [ideal solution](ideal-solution.md) made from pure [liquids](liquid.md) at the same [temperature](temperature-split.md) and [pressure](pressure-split.md), let $n=\sum_i n_i$. Then

$$
\Delta_{\rm mix}S=-R\sum_i n_i\ln x_i
=-nR\sum_i x_i\ln x_i.
$$

The right-hand expression is the [ideal solution](ideal-solution.md) result; the general definition does not require ideality. Each interior [mole fraction](mole-fraction.md) has a negative [logarithm](logarithm.md), so mixing distinct components gives positive [entropy of mixing](entropy-of-mixing.md). At a pure endpoint, use the [limit](limit-of-a-function.md) $x\ln x\to0$ as $x\to0^+$.

For one [mole](mole-unit.md) of the chosen A/B [ideal solution](ideal-solution.md) with $x_A=0.4$,

$$
-0.4\ln0.4-0.6\ln0.6\approx0.673011667,
\qquad
\Delta_{\rm mix}S\approx5.59573\,\mathrm{J\,K^{-1}}.
$$

For the same total [amount of substance](amount-of-substance.md), equal [mole fractions](mole-fraction.md) maximize this binary [entropy of mixing](entropy-of-mixing.md): the composition function $s(x)=-x\ln x-(1-x)\ln(1-x)$ has

$$
s'(x)=\ln\frac{1-x}{x},\qquad
s''(x)=-\frac{1}{x}-\frac{1}{1-x}<0,
$$

so its unique maximum is $s(1/2)=\ln2$. This is a comparison between different prepared compositions, not a prediction that a closed sample changes its component inventory to become equimolar.

**Table of contents**

- [Entropy of a two-species classical ideal gas](entropy-of-a-two-species-classical-ideal-gas.md)

## ↑ Ancestors (5)

1. [Ideal solution](ideal-solution.md)
2. [Solution (chemistry)](solution-chemistry.md)
3. [Mixture](mixture-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Entropy of mixing](entropy-of-mixing.md)
- [Flory–Huggins solution theory](flory-huggins-solution-theory.md)
- [Gibbs free energy of mixing](gibbs-free-energy-of-mixing.md)
- [Gibbs paradox](gibbs-paradox.md)
- [Ideal solution](ideal-solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2/a7/b/iii/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-a/a2/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-a/a2/b/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006/section-a/a2/d/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2017/4/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/6/a/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018/section-a/a1/c/solution.md)
- [Regular solution](regular-solution.md)
- [Symmetric Flory-Huggins polymer blend](symmetric-flory-huggins-polymer-blend.md)
