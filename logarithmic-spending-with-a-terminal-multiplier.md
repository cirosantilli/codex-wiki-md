# Logarithmic spending with a terminal multiplier

↑ **Parent:** [Optimal control](optimal-control.md)

For bank dynamics $\dot x=A+rx-u$ and utility $\int_0^T e^{-\beta t}\log u\,dt+\mu e^{-\beta T}x(T)$, substituting the terminal balance separates the concave optimization pointwise and gives the displayed control for $\mu>0$. Put $W=e^{rT}x(0)+A(e^{rT}-1)/r$ and $B=\int_0^T e^{\beta s}ds$. Its terminal balance is $W-B/\mu$, so the unique positive multiplier achieving zero terminal wealth is $B/W$. The same control solves the problem with no terminal reward and constraint $x(T)\ge0$, by the supporting-line inequality for logarithms.

## ↑ Ancestors (5)

1. [Optimal control](optimal-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/29i/solution.md)
