# Legendre symbol

↑ **Parent:** [Quadratic residue](quadratic-residue-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Legendre_symbol)

For an [integer](integer-split.md) $a$ and an **[odd prime](odd-prime.md)** $p$, the Legendre symbol is the [integer](integer-split.md) valued [function](function-split.md)

$$
\left(\frac ap\right)=
\begin{cases}
0,&p\mid a,\\
1,&a\not\equiv0\pmod p\text{ is a square},\\
-1,&a\text{ is a nonsquare}.
\end{cases}
$$

Its value depends only on the [congruence class](congruence-class.md) of $a$ modulo $p$; the displayed notation is a symbol, not division. The value zero handles $p\mid a$ separately from [quadratic residues](quadratic-residue-split.md) and [quadratic nonresidues](quadratic-nonresidue.md).[Ben Lynn, Quadratic Residues, The Legendre Symbol: three values and dependence on an odd prime](quadratic-residues-by-ben-lynn.md)

For example, $(2/7)=1$, $(3/7)=-1$, $(14/7)=0$, and $(2/11)=-1$. The equality $(9/7)=(2/7)=1$ illustrates that choosing a different [integer](integer-split.md) representative does not change the answer. An arbitrary odd composite denominator uses the [Jacobi symbol](jacobi-symbol.md), not the [Legendre symbol](legendre-symbol.md). For instance,

$$
\left(\frac2{15}\right)_{\!\mathrm{Jacobi}}
=\left(\frac23\right)\left(\frac25\right)=(-1)(-1)=1,
$$

but two is not a square modulo fifteen: any such [square root](square-root.md) would also give a [square root](square-root.md) modulo three, where the only nonzero square is one. A [Jacobi symbol](jacobi-symbol.md) of one therefore cannot replace the [Legendre symbol](legendre-symbol.md)'s square test.

The [Legendre symbol](legendre-symbol.md) also counts [square roots](square-root.md) compactly. For every [congruence class](congruence-class.md) $a$ in the [prime field](prime-field.md) $\mathbb F_p$,

$$
\#\{x\in\mathbb F_p:x^2=a\}=1+\left(\frac ap\right).
$$

The three cases give two, one and zero solutions for a [quadratic residue](quadratic-residue-split.md), zero and a [quadratic nonresidue](quadratic-nonresidue.md), respectively. This is useful when counting solutions of [modular congruences](modular-congruence.md) involving [polynomials](polynomial-split.md): a solvability question becomes a sum of [Legendre symbols](legendre-symbol.md), as in the [complete Legendre-symbol sum](complete-legendre-symbol-sum.md) and [quadratic Legendre-symbol correlation](quadratic-legendre-symbol-correlation.md).

**Table of contents**

- [Multiplicativity of the Legendre symbol](multiplicativity-of-the-legendre-symbol.md)
- [Complete Legendre-symbol sum](complete-legendre-symbol-sum.md)
- [Quadratic Legendre-symbol correlation](quadratic-legendre-symbol-correlation.md)
  - [Number of consecutive nonzero quadratic residues modulo an odd prime](number-of-consecutive-nonzero-quadratic-residues-modulo-an-odd-prime.md)
- [Euler's criterion](euler-s-criterion.md)
  - [Primes congruent to five modulo eight from odd squares plus four](primes-congruent-to-five-modulo-eight-from-odd-squares-plus-four.md)
- [Gauss's lemma (number theory)](gauss-s-lemma-number-theory.md)
- [Euler criterion](euler-criterion.md)
  - [First supplementary law for quadratic reciprocity](first-supplementary-law-for-quadratic-reciprocity.md)
  - [Second supplementary law for quadratic reciprocity](second-supplementary-law-for-quadratic-reciprocity.md)
    - [Euclid proof for infinitely many primes congruent to seven modulo eight](euclid-proof-for-infinitely-many-primes-congruent-to-seven-modulo-eight.md)
    - [Elementary logarithmic lower bound for primes in the quadratic-residue classes of two](elementary-logarithmic-lower-bound-for-primes-in-the-quadratic-residue-classes-of-two.md)
  - [Prime-power binomial congruence for a matrix](prime-power-binomial-congruence-for-a-matrix.md)
- [Weighted complete Legendre-symbol sum](weighted-complete-legendre-symbol-sum.md)
- [Lower-half quadratic-residue sum for primes congruent to seven modulo eight](lower-half-quadratic-residue-sum-for-primes-congruent-to-seven-modulo-eight.md)
- [Discriminant criterion for a quadratic congruence modulo an odd prime](discriminant-criterion-for-a-quadratic-congruence-modulo-an-odd-prime.md)

## ↑ Ancestors (5)

1. [Quadratic residue](quadratic-residue-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (48)

- [Coefficient formula for trace of Frobenius modulo p](coefficient-formula-for-trace-of-frobenius-modulo-p.md)
- [Computing Legendre symbols by quadratic reciprocity](computing-legendre-symbols-by-quadratic-reciprocity.md)
- [Euler's criterion](euler-s-criterion.md)
- [Explicit quadratic Hilbert symbols over the p-adic numbers](explicit-quadratic-hilbert-symbols-over-the-p-adic-numbers.md)
- [Infinitely many prime quadratic nonresidues of a nonsquare integer](infinitely-many-prime-quadratic-nonresidues-of-a-nonsquare-integer.md)
- [Lattice-point count for quadratic reciprocity](lattice-point-count-for-quadratic-reciprocity.md)
- [Legendre symbol](legendre-symbol.md)
- [Multiplicativity of the Legendre symbol](multiplicativity-of-the-legendre-symbol.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/17b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/19f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/17g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/17g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-21/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-23/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-7/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-26/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/11i/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-23/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-22/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/1h/solution.md)
- [9H](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/9h.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-26/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-125/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/11h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/11i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/11g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/1g/a/solution.md)
- [Point-count criterion for y squared equals x cubed plus k x](point-count-criterion-for-y-squared-equals-x-cubed-plus-k-x.md)
- [Quadratic Gauss sum](quadratic-gauss-sum.md)
- [Quadratic reciprocity](quadratic-reciprocity.md)
- [Quadratic residue](quadratic-residue-split.md)
- [Rational torsion of a congruent number curve](rational-torsion-of-a-congruent-number-curve.md)
- [Reduced positive definite binary quadratic forms of discriminant minus thirty-five](reduced-positive-definite-binary-quadratic-forms-of-discriminant-minus-thirty-five.md)
- [Vanishing trace criterion for a congruent number curve](vanishing-trace-criterion-for-a-congruent-number-curve.md)
