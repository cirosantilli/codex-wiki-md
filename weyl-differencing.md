# Weyl differencing

↑ **Parent:** [Exponential sum](exponential-sum.md)

Taking a [finite difference](finite-difference-split.md) lowers the degree of a polynomial phase. For $S(\theta)=\sum_{x=1}^n e(\theta P(x))$, expand $|S|^2$ by shifts $h$ and apply the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) to those shift sums. This gives $|S|^4\le2n\sum_{h,l}\sum_{x\in I_{h,l}}e(\theta\Delta_h\Delta_lP(x))$, where $I_{h,l}$ enforces that $x,x+h,x+l,x+h+l$ lie in $[1,n]$. Although individual terms can be complex, the entire sum is real and nonnegative because it equals a sum of squares. For $P(x)=x^3$, the phase is $3hl(2x+h+l)$.

**Table of contents**

- [Weyl inequality](weyl-inequality.md)
- [Cubic Weyl inequality](cubic-weyl-inequality.md)
- [Hua's lemma](hua-s-lemma.md)
  - [Cubic eighth-moment proof by differencing](cubic-eighth-moment-proof-by-differencing.md)

## ↑ Ancestors (6)

1. [Exponential sum](exponential-sum.md)
2. [Analytic number theory](analytic-number-theory-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Cubic eighth-moment proof by differencing](cubic-eighth-moment-proof-by-differencing.md)
- [Cubic Weyl inequality](cubic-weyl-inequality.md)
- [Hua's lemma](hua-s-lemma.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76/1/solution.md)
- [Uniform square recurrence on the circle](uniform-square-recurrence-on-the-circle.md)
- [Weyl inequality](weyl-inequality.md)
