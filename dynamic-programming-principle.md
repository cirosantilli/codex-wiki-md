# Dynamic programming principle

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

An optimal value over a time interval is the supremum of immediate reward plus the conditional optimal continuation value. For a controlled state $X$ and running reward $\ell$, this reads $J(x,t)=\sup_a\mathbb E[\int_t^{t+h}\ell(X_s,a_s,s)ds+J(X_{t+h},t+h)\mid X_t=x]$, under the usual admissible concatenation and information conditions. Conditioning and concatenating strategies proves both inequalities: every strategy's continuation is bounded by the value function, while approximately optimal continuations approach that bound. For a smooth diffusion value function, [Itô formula](ito-s-lemma.md) and the limit $h\downarrow0$ yield the [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md).

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/2/c/solution.md)
