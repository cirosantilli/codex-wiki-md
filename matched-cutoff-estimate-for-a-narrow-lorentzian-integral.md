# Matched cutoff estimate for a narrow Lorentzian integral

↑ **Parent:** [Matched asymptotic expansion](matched-asymptotic-expansion.md)

Split the [integral](integral-split.md) at $\epsilon\ll\delta\ll1$. Replacing the numerator by one below the cutoff gives $\epsilon^{-1}\arctan(\delta/\epsilon)$, with an error bounded by $\tfrac12\log(1+\delta^2/\epsilon^2)$. Above the cutoff, replacing the denominator by $x^2$ has relative error $O(\epsilon^2/\delta^2)$, and [integration by parts](integration-by-parts.md) gives $1/\delta+\log\delta+O(1)$. The inner $-1/\delta$ cancels the outer $1/\delta$, and all errors are $o(1/\epsilon)$, proving the leading constant independently of the intermediate cutoff.

## ↑ Ancestors (8)

1. [Matched asymptotic expansion](matched-asymptotic-expansion.md)
2. [Singular perturbation](singular-perturbation-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
