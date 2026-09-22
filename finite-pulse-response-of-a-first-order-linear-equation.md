# Finite-pulse response of a first-order linear equation

↑ **Parent:** [First-order linear differential equation](first-order-linear-differential-equation.md)

Let $0<a<b$ and $y'-\lambda y=A[H(t-a)-H(t-b)]$, with zero initial data. For $\lambda\ne0$, the [Laplace transform time-shift rule](laplace-transform-time-shift-rule.md) gives the displayed response, since the transform of the input is $A(e^{-as}-e^{-bs})/s$ and the equation supplies the factor $(s-\lambda)^{-1}$. Equivalently, integrate the [impulse response](impulse-response.md) $e^{\lambda t}H(t)$ over the active pulse. Before $a$ the solution is zero; during the pulse it is $A(e^{\lambda(t-a)}-1)/\lambda$; after $b$ it is $Ae^{\lambda t}(e^{-\lambda a}-e^{-\lambda b})/\lambda$. The solution is continuous at both switching times. At $\lambda=0$ take the [limit](limit-of-a-function.md), giving linear growth during the pulse and the constant $A(b-a)$ afterward. Positive $\lambda$ gives growing memory, while negative $\lambda$ gives decay after forcing stops.

## ↑ Ancestors (8)

1. [First-order linear differential equation](first-order-linear-differential-equation.md)
2. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/5/ii/solution.md)
