# Simpson multistep method

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

Integrating a quadratic interpolant of the derivative over two steps gives this [linear multistep method](linear-multistep-method.md), which has order four. Its [local truncation error](local-truncation-error.md) is $-h^5y^{(5)}(t_{n+1})/90+O(h^7)$ and its [zero-stability](zero-stability.md) polynomial is $\rho(\zeta)=\zeta^2-1$, with simple roots $1,-1$. The [Dahlquist equivalence theorem](dahlquist-equivalence-theorem.md) therefore gives fourth-order convergence with sufficiently accurate starts. This attains the even two-step [first Dahlquist barrier](first-dahlquist-barrier.md). Its undamped parasitic zero-step mode need not have favorable long-time [absolute stability](linear-stability-domain.md); finite-time convergence and stiff damping are separate requirements.

## ↑ Ancestors (6)

1. [Linear multistep method](linear-multistep-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/6/solution.md)
