# Strong Lagrangian property

↑ **Parent:** [Lagrangian duality](lagrangian-duality.md)

For a finite constrained optimum value $\phi(b)=\inf\{f(x):h(x)=b,x\in X\}$ and [optimization Lagrangian](optimization-lagrangian.md) $L_b(x,\lambda)=f(x)-\lambda^T(h(x)-b)$, the strong Lagrangian property means that some finite [Lagrange multiplier](lagrange-multiplier.md) attains the dual lower bound exactly: $\inf_XL_b=\phi(b)$. It includes dual attainment, but need not include primal attainment. It is equivalent to a [non-vertical supporting hyperplane of a value function](non-vertical-supporting-hyperplane-of-a-value-function.md): a supporting slope gives $f(x)\geq\phi(h(x))\geq\phi(b)+\lambda^T(h(x)-b)$, hence $\inf_XL_b\geq\phi(b)$; [weak duality](weak-duality.md) gives the opposite inequality. Conversely the infimum identity bounds every $L_b(x,\lambda)$ below by $\phi(b)$; taking the infimum over $h(x)=u$ gives the supporting inequality. No convexity assumption is needed for this equivalence.

## ↑ Ancestors (5)

1. [Lagrangian duality](lagrangian-duality.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Non-vertical supporting hyperplane of a value function](non-vertical-supporting-hyperplane-of-a-value-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/1/solution.md)
