# Square root of a CIR diffusion

↑ **Parent:** [Cox–Ingersoll–Ross model](cox-ingersoll-ross-model.md)

For $dC_t=a(b-C_t)dt+\sigma\sqrt{C_t}\,dW_t$, the [Itô formula](ito-s-lemma.md) applied to $Z=\sqrt C$ gives the displayed dynamics before hitting zero. In particular $2ab=\sigma^2$ does not eliminate the reciprocal drift. The cancellation condition is $4ab=\sigma^2$. Under that condition $C$ can be represented as the square of a signed [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md) with drift $-aY/2$ and volatility $\sigma/2$; its principal square root is the reflected process $|Y|$, not an unrestricted signed OU process. The mean of $C$ is $b+(C_0-b)e^{-at}$ for all admissible positive parameters.

## ↑ Ancestors (9)

1. [Cox–Ingersoll–Ross model](cox-ingersoll-ross-model.md)
2. [Short rate](short-rate.md)
3. [Interest rate](interest-rate.md)
4. [Fixed-income security](fixed-income-security.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/1/solution.md)
