# Asymptotic analysis

↑ **Parent:** [Real analysis](real-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_analysis)

Asymptotic analysis describes what remains dominant as an argument approaches a specified [limit](limit-of-a-function.md). It compares [functions](function-split.md) or [sequences](sequence.md) by scale: how much of a complicated expression can be replaced by a simpler one, and how large is the omitted part? The [limit](limit-of-a-function.md) may be $n\to\infty$ for a growing input or $h\to0$ for a shrinking approximation parameter.

For example, $n^2+10^5n$ is eventually dominated by its quadratic term, since division by $n^2$ gives $1+10^5/n\to1$. But at $n=100$, the linear term contributes $10^7$, compared with only $10^4$ from the quadratic term. A statement about the limiting scale and a good approximation at a particular input are different claims.

Three useful comparisons keep their strengths distinct. [Big O notation](big-o-notation.md) supplies an eventual [upper bound](upper-bound-in-a-partially-ordered-set.md) up to a constant multiplier; [big theta notation](big-theta-notation.md) supplies both an [upper bound](upper-bound-in-a-partially-ordered-set.md) and a [lower bound](lower-bound-in-a-partially-ordered-set.md) up to constants; [asymptotic equivalence](asymptotic-equivalence.md) makes the ratio tend to one. [Little o notation](little-o-notation.md) says that a term becomes negligible relative to a specified scale. These distinctions make approximations checkable instead of merely calling one expression small.

The same language connects [time complexity](time-complexity.md) with [Taylor remainders](taylor-remainder.md). In an operation-count model, one asks how a cost scales with input size. In a [Taylor expansion](taylor-expansion.md), one asks how the approximation error scales with the increment. Neither use requires interpreting the unspecified constant as one. The [asymptotic comparison of exponential functions](asymptotic-comparison-of-exponential-functions.md) gives another example: dividing by the largest contributing exponential reveals the terms that disappear.

**Table of contents**

- [Asymptotic equivalence](asymptotic-equivalence.md)
  - [Asymptotic comparison of exponential functions](asymptotic-comparison-of-exponential-functions.md)
  - [Stirling formula](stirling-formula.md)
    - [Robbins bounds for Stirling's formula](robbins-bounds-for-stirling-s-formula.md)
    - [Gaussian peak behind Stirling's formula](gaussian-peak-behind-stirling-s-formula.md)
    - [Stirling correction by Gaussian moments](stirling-correction-by-gaussian-moments.md)

## ↑ Ancestors (5)

1. [Real analysis](real-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Karatsuba operand splitting](karatsuba-operand-splitting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-45/3/solution.md)
