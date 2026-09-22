# Zoutendijk theorem

↑ **Parent:** [Line search](line-search.md)

Suppose $f$ is bounded below on its initial level set, continuously differentiable with a Lipschitz gradient nearby, and each [descent direction](descent-direction.md) $p_k$ uses a step satisfying fixed [Wolfe conditions](wolfe-conditions.md). If $\cos\theta_k=-\nabla f(x_k)^Tp_k/(\|\nabla f(x_k)\|\|p_k\|)$, the displayed series converges. In particular a uniform positive lower bound on these cosines gives $\nabla f(x_k)\to0$.

For a gradient Lipschitz constant $L$, the curvature condition gives $\alpha_k\geq(1-\eta)(-\nabla f^Tp_k)/(L\|p_k\|^2)$. Sufficient decrease then gives $f(x_k)-f(x_{k+1})\geq\sigma(1-\eta)\cos^2\theta_k\|\nabla f(x_k)\|^2/L$. Summing and using the lower bound on $f$ proves the assertion.

## ↑ Ancestors (5)

1. [Line search](line-search.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/2/ii/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/2/iii/solution.md)
