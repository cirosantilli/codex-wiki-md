# Quadratic residue

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_residue)

For an [odd prime](odd-prime.md) $p$, a nonzero [congruence class](congruence-class.md) $a$ is a quadratic residue when $a\equiv x^2\pmod p$ for some [integer](integer-split.md) $x$. Here **"quadratic residue" excludes zero**: zero is a [square of a number](square-of-a-number.md), but is neither a [quadratic residue](quadratic-residue-split.md) nor a [quadratic nonresidue](quadratic-nonresidue.md) under this convention. Some treatments include zero among [quadratic residues](quadratic-residue-split.md); the distinction matters when counting them or discussing their [subgroup](subgroup.md).[Keith Conrad, Quadratic Residue Patterns Modulo a Prime, §1, p. 1: nonzero convention and equal counts](quadratic-residue-patterns-modulo-a-prime-by-keith-conrad.md)

Modulo seven, squaring the six nonzero [congruence classes](congruence-class.md) gives

$$
\begin{array}{c|rrrrrr}
x&1&2&3&4&5&6\\\hline
x^2\bmod7&1&4&2&2&4&1
\end{array}
$$

Thus the [set](set-split.md) of [quadratic residues](quadratic-residue-split.md) is $Q_7=\{1,2,4\}$, and the [quadratic nonresidues](quadratic-nonresidue.md) are $\{3,5,6\}$. In particular, **$x^2\equiv2\pmod7$ has exactly the two solutions $x\equiv3,4\pmod7$**: $3^2=9\equiv2$ and $4^2=16\equiv2$. Modulo eleven the [quadratic residues](quadratic-residue-split.md) are instead $Q_{11}=\{1,3,4,5,9\}$. Two is therefore a [quadratic residue](quadratic-residue-split.md) modulo seven and a [quadratic nonresidue](quadratic-nonresidue.md) modulo eleven: being a [quadratic residue](quadratic-residue-split.md) depends on the modulus.

<a id="image-the-square-map-modulo-seven-and-eleven-two-inputs-in-every-nonzero-square-fiber"></a>
![](quadratic-residue-square-map-fibers.png)

**[Figure 1](#image-the-square-map-modulo-seven-and-eleven-two-inputs-in-every-nonzero-square-fiber). The square map modulo seven and eleven: two inputs in every nonzero square fiber**. Each pair $\{x,p-x\}$ maps to one [quadratic residue](quadratic-residue-split.md). The six nonzero inputs modulo seven give three outputs; the ten modulo eleven give five. The zero [fiber](fiber-of-a-function.md) is the single input zero, and each [quadratic nonresidue](quadratic-nonresidue.md) has an empty [fiber](fiber-of-a-function.md).

Why do the [square roots](square-root.md) come in pairs? If $x^2\equiv y^2\pmod p$, the [prime number](prime-number-split.md) $p$ divides $(x-y)(x+y)$, so it divides one factor: $y\equiv x$ or $y\equiv-x\pmod p$. For nonzero $x$ these are distinct, because $p$ is an [odd prime](odd-prime.md). Every nonempty nonzero [fiber of a function](fiber-of-a-function.md) of $s(x)=x^2$ therefore contains exactly two inputs. Pairing the $p-1$ nonzero [congruence classes](congruence-class.md) gives exactly $(p-1)/2$ [quadratic residues](quadratic-residue-split.md) and $(p-1)/2$ [quadratic nonresidues](quadratic-nonresidue.md). Including zero gives $(p+1)/2$ different squares, with one rather than two [square roots](square-root.md) for zero.

The [quadratic residues](quadratic-residue-split.md) form a [subgroup](subgroup.md) of the [multiplicative group of a finite field](multiplicative-group-of-a-finite-field.md) $\mathbb F_p^\times$, with [index of a subgroup](index-of-a-subgroup.md) two. Indeed, one is a square, $(u^2)(v^2)=(uv)^2$, and $(u^2)^{-1}=(u^{-1})^2$; the inverses exist because the inputs are nonzero in the [prime field](prime-field.md). Equivalently, the squaring [group homomorphism](group-homomorphism.md) has [kernel of a group homomorphism](kernel-of-a-group-homomorphism.md) $\{1,-1\}$ and [image of a function](image-of-a-function.md) $Q_p$. The apparent loss of a sign in squaring becomes a precise division of the nonzero arithmetic into two equal parts.

This structure turns a search for [square roots](square-root.md) into a yes-or-no test: [Euler's criterion](euler-s-criterion.md) detects [quadratic residues](quadratic-residue-split.md) through [modular exponentiation](modular-exponentiation.md), and the [Legendre symbol](legendre-symbol.md) records the result as a sign. For a general [integer](integer-split.md) modulus, the [modular congruence](modular-congruence.md) $x^2\equiv a\pmod n$ still makes sense, but the two-root count and the [prime field](prime-field.md) argument need not survive. For example, $x^2\equiv1\pmod{15}$ has four solutions $1,4,11,14$; the [Chinese remainder theorem](chinese-remainder-theorem.md) separates the sign choices modulo three and five.

**Table of contents**

- [Square root of minus one modulo a prime](square-root-of-minus-one-modulo-a-prime.md)
- [Quadratic nonresidue](quadratic-nonresidue.md)
  - [Least quadratic nonresidue](least-quadratic-nonresidue.md)
    - [Large-sieve logarithmic exceptional-prime bound for least quadratic nonresidues](large-sieve-logarithmic-exceptional-prime-bound-for-least-quadratic-nonresidues.md)
    - [Bounded exceptional primes for least quadratic nonresidues](bounded-exceptional-primes-for-least-quadratic-nonresidues.md)
- [Quadratic Gauss sum](quadratic-gauss-sum.md)
  - [Quadratic periods modulo eleven](quadratic-periods-modulo-eleven.md)
- [Legendre symbol](legendre-symbol.md)
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

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (43)

- [Bounded exceptional primes for least quadratic nonresidues](bounded-exceptional-primes-for-least-quadratic-nonresidues.md)
- [Computing Legendre symbols by quadratic reciprocity](computing-legendre-symbols-by-quadratic-reciprocity.md)
- [Euler's criterion](euler-s-criterion.md)
- [Jacobi reciprocity law](jacobi-reciprocity-law.md)
- [Legendre symbol](legendre-symbol.md)
- [Multiplicativity of the Legendre symbol](multiplicativity-of-the-legendre-symbol.md)
- [Noncongruent primes congruent to three modulo eight](noncongruent-primes-congruent-to-three-modulo-eight.md)
- [Obstruction to norm-minus-one units from a prime congruent to three modulo four](obstruction-to-norm-minus-one-units-from-a-prime-congruent-to-three-modulo-four.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-19/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-21/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/20g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/1g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/1g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-23/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/6e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/9h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/18h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-125/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/5e/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-114/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/11i/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/1g/solution.md)
- [Prime representation when h of minus eight q equals two](prime-representation-when-h-of-minus-eight-q-equals-two.md)
- [Quadratic nonresidue](quadratic-nonresidue.md)
- [Quadratic reciprocity](quadratic-reciprocity.md)
- [Quadratic residue](quadratic-residue-split.md)
- [Signed divisor-two obstruction for an isogeny covering](signed-divisor-two-obstruction-for-an-isogeny-covering.md)
- [Stronger prime-divisor congruence for Fermat numbers](stronger-prime-divisor-congruence-for-fermat-numbers.md)
- [Tonelli-Shanks algorithm](tonelli-shanks-algorithm.md)
