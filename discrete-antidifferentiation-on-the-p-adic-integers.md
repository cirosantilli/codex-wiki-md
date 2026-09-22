# Discrete antidifferentiation on the p-adic integers

↑ **Parent:** [Mahler's theorem](mahler-s-theorem.md)

The [Mahler coefficients](mahler-coefficient.md) tend to zero, so the displayed series defines a [continuous function](continuous-function.md) and has value zero at zero. The [Pascal's identity](pascal-s-rule.md) and uniform convergence give $\Delta Jf=f$. Thus the [forward difference operator](forward-difference-operator.md) is surjective on [continuous functions on the p-adic integers](continuous-functions-on-the-p-adic-integers.md). Its kernel consists of constants: period one implies agreement on the dense nonnegative integers, and [continuity](continuous-function.md) then implies constancy. This selects the unique [discrete antiderivative](discrete-antiderivative.md) vanishing at zero.

There is also a direct construction on [locally constant functions](locally-constant-function.md). If $h$ has period $M=p^r$, put $a_j=h(j)$, $S=\sum_{i=0}^{M-1}a_i$, and $P_j=\sum_{i<j}a_i$. For $x=j+My$ with $0\le j<M$ and $y\in\mathbb Z_p$, set

$$
Jh(x)=yS+P_j.
$$

This is a [continuous function](continuous-function.md) on each residue class. Increasing $j$ gives $Jh(x+1)-Jh(x)=a_j$; at $j=M-1$, the next point has residue zero and quotient $y+1$, giving the same identity. The [ultrametric inequality](ultrametric-inequality.md) gives $\|Jh\|_\infty\le\|h\|_\infty$, and $Jh(0)=0$. The construction is independent of the chosen period, since two normalized [discrete antiderivatives](discrete-antiderivative.md) agree on the nonnegative integers and then on the [p-adic integers](p-adic-integer.md) by [continuity](continuous-function.md). It is linear on the [locally constant functions](locally-constant-function.md), which form a [dense subset](dense-set.md) in the [supremum norm](supremum-norm.md). Completeness therefore extends it to every [continuous function](continuous-function.md), retaining $\Delta J=I$ and the norm bound. This proves surjectivity without first using the [Mahler theorem](mahler-s-theorem.md).

**Table of contents**

- [Translation-invariant linear forms on p-adic continuous functions vanish](translation-invariant-linear-forms-on-p-adic-continuous-functions-vanish.md)

## ↑ Ancestors (7)

1. [Mahler's theorem](mahler-s-theorem.md)
2. [Continuous functions on the p-adic integers](continuous-functions-on-the-p-adic-integers.md)
3. [Non-Archimedean analysis](non-archimedean-analysis.md)
4. [Arithmetic](arithmetic-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-27/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-136/2/solution.md)
