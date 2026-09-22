# Gradient ascent pulse engineering

↑ **Parent:** [Quantum optimal control](quantum-optimal-control.md)

[Gradient ascent pulse engineering](gradient-ascent-pulse-engineering.md) parametrizes each control by time-slice amplitudes and optimizes a differentiable quantum-control objective. Forward products of slice [unitary operators](unitary-operator.md) and backward adjoint propagation give derivatives with respect to every amplitude. For $U_j=e^{-iH_j\Delta t}$, the exact derivative is $\partial_{f_m}U_j=-i\int_0^{\Delta t}e^{-iH_j(\Delta t-\tau)}H_m e^{-iH_j\tau}\,d\tau$. Updating all slice amplitudes along these derivatives is gradient ascent for a fidelity, or gradient descent for its negative.

## ↑ Ancestors (6)

1. [Quantum optimal control](quantum-optimal-control.md)
2. [Optimal control](optimal-control.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Gradient ascent pulse engineering](gradient-ascent-pulse-engineering.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/1/d/solution.md)
