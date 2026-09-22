# Strong stability preserving Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

A strong stability preserving Runge-Kutta method writes its stages as convex combinations of previously computed states and suitable [Forward Euler method](euler-method.md) steps. It transfers any convex-functional nonincrease property of the forward step, such as a [norm](norm.md) bound, under a proportionally scaled time-step restriction.

For example, if $E_k(U)=U+kF(U)$ is nonexpansive in a [norm](norm.md), then $Y=E_k(U)$ and $U_{\mathrm{new}}=(U+E_k(Y))/2$ is also nonexpansive: the [triangle inequality](triangle-inequality.md) bounds the new difference by one half of the initial difference plus one half of the twice-advanced difference. Both are at most the initial difference. A [Taylor expansion](taylor-expansion.md) yields $U_{\mathrm{new}}=U+kF(U)+k^2F'(U)F(U)/2+O(k^3)$, so this is a second-order [Runge-Kutta method](runge-kutta-method.md). The forward-step hypothesis must hold on the stage states; preservation of one chosen convex bound is not the same as unconditional [B-stability](b-stability.md).

## ↑ Ancestors (6)

1. [Runge-Kutta method](runge-kutta-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
