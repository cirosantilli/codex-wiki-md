# Ill-posedness of numerical differentiation

↑ **Parent:** [Numerical differentiation](numerical-differentiation.md)

Recovering a [derivative](derivative.md) from values controlled only in the [uniform norm](supremum-norm.md) is an [ill-posed problem](ill-posed-problem.md): the differentiation map is not [continuous](continuous-function.md) in those norms. On $[0,1]$, take $f_k(x)=\sin(kx)/k$. Then $\|f_k\|_\infty\leq1/k\to0$, while $f_k'(x)=\cos(kx)$ has [uniform norm](supremum-norm.md) one for every $k$. Arbitrarily small value perturbations can therefore conceal nonvanishing [derivative](derivative.md) changes.

[Numerical differentiation](numerical-differentiation.md) can still be useful when additional smoothness bounds, a suitable sampling scale, or a [regularization](regularization.md) method control the admissible changes. The basic [noise amplification by differentiation of a linear interpolant](noise-amplification-by-differentiation-of-a-linear-interpolant.md) gives a finite-data version: endpoint uncertainty of size $\delta$ produces [derivative](derivative.md) uncertainty of order $\delta/h$ at spacing $h$.

**Table of contents**

- [Noise amplification by differentiation of a linear interpolant](noise-amplification-by-differentiation-of-a-linear-interpolant.md)

## ↑ Ancestors (6)

1. [Numerical differentiation](numerical-differentiation.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Numerical differentiation](numerical-differentiation.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2015/2/c/iii/solution.md)
