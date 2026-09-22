# Cauchy decrease bound

↑ **Parent:** [Cauchy point](cauchy-point.md)

Use the induced [spectral norm](matrix-2-norm.md) for the [symmetric matrix](symmetric-matrix.md) $H$ and interpret $\|g\|/\|H\|=+\infty$ when $H=0$. If $q=g^THg\leq0$, the [Cauchy point](cauchy-point.md) gives a decrease at least $\Delta\|g\|$. If $q>0$, its [step size](step-size.md) satisfies $\tau q\leq\|g\|^2$ and $q\leq\|H\|\|g\|^2$, so

$$
m(0)-m(s_C)=\tau\|g\|^2-\tfrac12\tau^2q\geq\tfrac12\tau\|g\|^2\geq\tfrac12\|g\|\min\{\Delta,\|g\|/\|H\|\}.
$$

Thus the numerical constant $1/2$ is independent of the model data. The bound links a nonzero [gradient](gradient.md) to a definite predicted decrease, including for an [indefinite matrix](indefinite-matrix.md) $H$.

**Table of contents**

- [Fraction of Cauchy decrease](fraction-of-cauchy-decrease.md)

## ↑ Ancestors (7)

1. [Cauchy point](cauchy-point.md)
2. [Trust-region subproblem](trust-region-subproblem.md)
3. [Trust region](trust-region.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Fraction of Cauchy decrease](fraction-of-cauchy-decrease.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/i/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/5/ii/solution.md)
- [Trust-region subproblem](trust-region-subproblem.md)
