# P-adic number

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P-adic_number)

For a [prime number](prime-number-split.md) $p$, a p-adic number is an element of the [field](field.md) $\mathbb Q_p$ obtained by completing the [rational numbers](rational-number.md) for the [metric](metric.md) $d_p(x,y)=|x-y|_p$. Here $|\cdot|_p$ is the [p-adic absolute value](p-adic-absolute-value.md). The [Cauchy-sequence construction of a metric completion](cauchy-sequence-construction-of-a-metric-completion.md) supplies limits for every [Cauchy sequence](cauchy-sequence.md), and [addition](addition.md), [multiplication](multiplication.md), and the [p-adic absolute value](p-adic-absolute-value.md) extend to this [complete metric space](complete-metric-space.md). The [rational numbers](rational-number.md) form a [dense subset](dense-set.md). [Stephen William Semmes, Notes on p-adic numbers, pages 4-5](https://arxiv.org/pdf/math/0502560)

For a concrete example with $p=2$, consider the [partial sums](partial-sum.md) of a [geometric series](geometric-series.md):

$$
s_n=\sum_{k=0}^{n-1}2^k=2^n-1,\qquad |s_n-(-1)|_2=|2^n|_2=2^{-n}.
$$

The first values $1,3,7,15,31$ have distances $1/2,1/4,1/8,1/16,1/32$ from $-1$ in the [2-adic absolute value](2-adic-absolute-value.md). Consequently

$$
-1=\sum_{k=0}^{\infty}2^k\qquad\text{in }\mathbb Q_2.
$$

This is a statement about [convergence in a metric space](convergence-in-a-metric-space.md) with the [2-adic absolute value](2-adic-absolute-value.md). In the ordinary [real number](real-number.md) [absolute value](absolute-value.md), the same [partial sums](partial-sum.md) grow without bound. Choosing a [metric](metric.md) changes which approximation errors shrink.

More generally every nonzero [P-adic number](p-adic-number.md) has a unique digit expansion

$$
x=\sum_{k=m}^{\infty}a_kp^k,\qquad m\in\mathbb Z,\quad a_m\ne0,\quad a_k\in\{0,1,\ldots,p-1\}.
$$

Only finitely many negative powers occur, while positive powers can continue indefinitely. Written with the highest powers on the left, the digits extend infinitely to the left; for example the [P-adic number](p-adic-number.md) $-1$ at $p=2$ is written $\ldots111_2$. The [p-adic integers](p-adic-integer.md) are exactly the elements with $|x|_p\leq1$, whose digit expansions use only nonnegative powers. [Andrew V. Sutherland, Number Theory I, Lecture 8, section 8.2, Proposition 8.17](https://math.mit.edu/classes/18.785/2021fa/LectureNotes8.pdf)

The construction can be understood through [modular arithmetic](modular-arithmetic-split.md). Successively choose the low-order digits to agree modulo $p$, $p^2$, and higher powers. After fixing digits below $p^n$, the remaining error has [p-adic absolute value](p-adic-absolute-value.md) at most $p^{-n}$; the [partial sums](partial-sum.md) form a [Cauchy sequence](cauchy-sequence.md), so completeness supplies a limit. If two expansions first differ at position $j$, their difference has [P-adic valuation](p-adic-valuation.md) $j$, proving uniqueness. This turns compatible finite [congruence classes](congruence-class.md) into one exact [number](number.md). In particular, [Hensel's lemma](hensel-s-lemma.md) upgrades suitable approximate [roots of a polynomial](root-of-a-polynomial.md) modulo powers of $p$ into roots in the [p-adic integers](p-adic-integer.md).

**Table of contents**

- [3-adic number](3-adic-number.md)
- [p-adic absolute value](p-adic-absolute-value.md)
  - [p-adic metric](p-adic-metric.md)
  - [2-adic absolute value](2-adic-absolute-value.md)
    - [2-adic metric](2-adic-metric.md)
  - [Ostrowski's theorem](ostrowski-s-theorem.md)
    - [Non-Archimedean part of Ostrowski theorem](non-archimedean-part-of-ostrowski-theorem.md)
    - [Non-Archimedean absolute values on a number field](non-archimedean-absolute-values-on-a-number-field.md)

## ↑ Ancestors (5)

1. [Non-Archimedean analysis](non-archimedean-analysis-split.md)
2. [Arithmetic](arithmetic-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (14)

- [2-adic absolute value](2-adic-absolute-value.md)
- [Continuous functions on the p-adic integers](continuous-functions-on-the-p-adic-integers.md)
- [Embedding of a number field into a p-adic algebraic closure](embedding-of-a-number-field-into-a-p-adic-algebraic-closure.md)
- [Hasse-Minkowski theorem](hasse-minkowski-theorem.md)
- [P-adic field](p-adic-field.md)
- [p-adic integer](p-adic-integer.md)
- [p-adic metric](p-adic-metric.md)
- [P-adic number](p-adic-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-27/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-29/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-28/1/b/ii/solution.md)
- [Ramification bound for a primitive pth root of unity](ramification-bound-for-a-primitive-pth-root-of-unity.md)
- [Rational Tate module](rational-tate-module.md)
- [Ultrametric space](ultrametric-space.md)
