# Cauchy point

↑ **Parent:** [Trust-region subproblem](trust-region-subproblem.md)

For $g\ne0$, the [Cauchy point](cauchy-point.md) minimizes the quadratic model along the feasible part of the negative [gradient](gradient.md) ray. Writing $q=g^THg$, its [step size](step-size.md) is

$$
\tau=\begin{cases}\Delta/\|g\|,&q\leq0,\\\min\{\Delta/\|g\|,\|g\|^2/q\},&q>0.\end{cases}
$$

Indeed $m(-tg)=a-t\|g\|^2+\tfrac12t^2q$ on $0\leq t\leq\Delta/\|g\|$. For $q\leq0$ it decreases throughout that interval; otherwise its unconstrained [minimum](minimum-of-a-subset-of-a-total-order.md) occurs at $t=\|g\|^2/q$. The constant $a$ does not affect the minimizing step.

**Table of contents**

- [Cauchy decrease bound](cauchy-decrease-bound.md)
  - [Fraction of Cauchy decrease](fraction-of-cauchy-decrease.md)

## ↑ Ancestors (6)

1. [Trust-region subproblem](trust-region-subproblem.md)
2. [Trust region](trust-region.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Cauchy decrease bound](cauchy-decrease-bound.md)
- [Cauchy point](cauchy-point.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/i/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/5/i/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/5/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/5/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/5/v/solution.md)
