# p-adic absolute value

↑ **Parent:** [P-adic number](p-adic-number.md)

Fix a [prime number](prime-number-split.md) $p$. Write a nonzero [rational number](rational-number.md) as $x=p^k a/b$, where $k\in\mathbb Z$ and the nonzero [integers](integer-split.md) $a,b$ are not divisible by $p$. The exponent $k$ is uniquely determined. Its [P-adic valuation](p-adic-valuation.md) is this signed exponent $v_p(x)=k$: equivalently, for any nonzero integer [numerator](numerator.md) $A$ and [denominator](denominator.md) $B$,

$$
v_p(A/B)=v_p(A)-v_p(B),\qquad |x|_p=p^{-v_p(x)},\qquad |0|_p=0.
$$

Factors of $p$ in the [numerator](numerator.md) decrease the [p-adic absolute value](p-adic-absolute-value.md); factors in the [denominator](denominator.md) increase it. For $p=2$ the computations are:

| [Rational number](rational-number.md) $x$ | Factorization | [P-adic valuation](p-adic-valuation.md) $v_2(x)$ | [2-adic absolute value](2-adic-absolute-value.md) $|x|_2$ |
| --- | --- | --- | --- |
| $8$ | $2^3$ | $3$ | $1/8$ |
| $12$ | $2^2\cdot3$ | $2$ | $1/4$ |
| $3/8$ | $2^{-3}\cdot3$ | $-3$ | $8$ |
| $-7$ | $2^0\cdot(-7)$ | $0$ | $1$ |
| $0$ | Not applicable | $+\infty$ by convention | $0$ |

This is an [absolute value on a field](absolute-value-algebra.md) measuring [divisibility](divisibility-split.md), rather than the magnitude on a [real number](real-number.md) [number line](number-line.md). It satisfies

$$
|xy|_p=|x|_p|y|_p,\qquad |x+y|_p\leq\max\{|x|_p,|y|_p\}.
$$

The proof comes directly from [P-adic valuations](p-adic-valuation.md): exponents add in a [product of numbers](product-of-numbers.md), and extracting a common power of $p$ from a [sum](sum.md) gives $v_p(x+y)\geq\min\{v_p(x),v_p(y)\}$. If the two [P-adic valuations](p-adic-valuation.md) differ, the remaining term with smaller exponent cannot cancel modulo $p$, so equality holds. Thus the [p-adic absolute value](p-adic-absolute-value.md) is a [Non-Archimedean absolute value](non-archimedean-absolute-value.md). [Stephen William Semmes, Notes on p-adic numbers, page 1](https://arxiv.org/pdf/math/0502560)

The [metric](metric.md) $d_p(x,y)=|x-y|_p$ makes two [rational numbers](rational-number.md) close when their difference contains a high power of $p$. This packages successive [modular congruences](modular-congruence.md) into a numerical error estimate, allowing [convergence in a metric space](convergence-in-a-metric-space.md) and [convergent series](convergent-series.md) to encode exact [arithmetic](arithmetic-split.md) information.

**Table of contents**

- [p-adic metric](p-adic-metric.md)
- [2-adic absolute value](2-adic-absolute-value.md)
  - [2-adic metric](2-adic-metric.md)
- [Ostrowski's theorem](ostrowski-s-theorem.md)
  - [Non-Archimedean part of Ostrowski theorem](non-archimedean-part-of-ostrowski-theorem.md)
  - [Non-Archimedean absolute values on a number field](non-archimedean-absolute-values-on-a-number-field.md)

## ↑ Ancestors (6)

1. [P-adic number](p-adic-number.md)
2. [Non-Archimedean analysis](non-archimedean-analysis-split.md)
3. [Arithmetic](arithmetic-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [2-adic absolute value](2-adic-absolute-value.md)
- [3-adic number](3-adic-number.md)
- [Embedding of a number field into a p-adic algebraic closure](embedding-of-a-number-field-into-a-p-adic-algebraic-closure.md)
- [Height of a rational number](height-of-a-rational-number.md)
- [Non-Archimedean place of a number field](non-archimedean-place-of-a-number-field.md)
- [p-adic absolute value](p-adic-absolute-value.md)
- [P-adic field](p-adic-field.md)
- [p-adic integer](p-adic-integer.md)
- [p-adic metric](p-adic-metric.md)
- [P-adic number](p-adic-number.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-28/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-21/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-24/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-123/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-145/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-136/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-166/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-136/1/c/solution.md)
- [Ultrametric space](ultrametric-space.md)
