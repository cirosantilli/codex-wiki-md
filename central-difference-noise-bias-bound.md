# Central-difference noise-bias bound

↑ **Parent:** [Linear regularization](linear-regularization.md)

For the mixed forward, [central finite difference](central-finite-difference.md), and backward derivative regularizer on $[0,1]$, with dividing points $(1-\alpha)/2$ and $(1+\alpha)/2$, the [overlap multiplicity bound for piecewise difference operators](overlap-multiplicity-bound-for-piecewise-difference-operators.md) has $m=3$. On the middle interval, the error kernel is $\operatorname{sgn}(s)(\alpha/2-|s|)/\alpha$ for $|s|\leq\alpha/2$, with [L1 norm](l1-norm.md) $\alpha/4$. [Young's convolution inequality](young-s-convolution-inequality.md) bounds that part of the bias by $\alpha\|f''\|_2/4$. If the two outer intervals together have squared error at most $\alpha^2\|f''\|_2^2$, combining the three pieces gives the displayed estimate for $\|f''\|_2\leq c$ and $\|f^\delta-f\|_2\leq\delta$. Interpreting $f'$ as the inverse of the [Volterra integration operator](volterra-operator.md) requires the [range of the Volterra integration operator](range-of-the-volterra-integration-operator.md) boundary condition $f(0)=0$.

## ↑ Ancestors (7)

1. [Linear regularization](linear-regularization.md)
2. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/1/v/solution.md)
