# Interval arithmetic

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interval_arithmetic)

[Interval arithmetic](interval-arithmetic.md) calculates with [closed intervals](closed-real-interval.md) that contain the possible values of a quantity. If all we know is $x\in X=[a,b]$, an [interval enclosure](interval-enclosure.md) for a [function](function-split.md) $f$ must contain $f(x)$ for every allowed $x$. The result says what is guaranteed, including uncertainty in the input and, with [outward rounding](outward-rounding.md), [roundoff error](round-off-error.md) in the calculation. A wide answer can still be correct; a narrow answer is useful only if it contains every possible value.

The attraction is that a finite calculation can make a statement about infinitely many [real numbers](real-number.md) at once. An [interval enclosure](interval-enclosure.md) can certify that a [function](function-split.md) stays positive throughout a whole [closed interval](closed-real-interval.md), or bound its [maximum](maximum-of-a-subset-of-a-total-order.md) for [mathematical optimization](mathematical-optimization-split.md). For example, on $X=[0,1]$, the actual [image of a function](image-of-a-function.md) for $f(x)=x(1-x)$ is $[0,1/4]$, but direct [interval arithmetic](interval-arithmetic.md) gives the wider $[0,1]$. [Interval subdivision](interval-subdivision.md) and the [interval square range](interval-square-range.md) improve this answer in different ways.

Historically, Ramon E. Moore's 1962 Stanford dissertation studied [interval arithmetic](interval-arithmetic.md) and automatic error analysis in digital computing; his book _Interval Analysis_ followed in 1966. Eldon Hansen's account documents earlier reports as well: these dates describe important steps in developing and disseminating the subject, rather than a claim of sole invention in a particular year.[Eldon R. Hansen, Publications Related to Early Interval Work of R. E. Moore, 2001, references 5 and 8](https://interval.louisiana.edu/Moores_early_papers/bibliography.html) Moore, R. Baker Kearfott and Michael J. Cloud later wrote _Introduction to Interval Analysis_ (2009).[R. Baker Kearfott, Books written or edited, entry for Introduction to Interval Analysis](https://interval.louisiana.edu/books.html)

**Table of contents**

- [Interval enclosure](interval-enclosure.md)
- [Interval arithmetic operations](interval-arithmetic-operations.md)
  - [Natural interval extension](natural-interval-extension.md)
    - [Interval dependency problem](interval-dependency-problem.md)
      - [Interval subdivision](interval-subdivision.md)
  - [Interval square range](interval-square-range.md)
- [Outward rounding](outward-rounding.md)
- [Interval root exclusion](interval-root-exclusion.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Axis-aligned bounding box](axis-aligned-bounding-box.md)
- [Interval arithmetic](interval-arithmetic.md)
- [Interval dependency problem](interval-dependency-problem.md)
- [Interval enclosure](interval-enclosure.md)
- [Interval root exclusion](interval-root-exclusion.md)
- [Lanford contraction proof of the Feigenbaum fixed point](lanford-contraction-proof-of-the-feigenbaum-fixed-point.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-53/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/6/solution.md)
