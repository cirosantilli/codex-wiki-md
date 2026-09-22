# Gaussian caplet bond-put formula

↑ **Parent:** [Caplet](caplet.md)

For a [Gaussian forward-rate field](gaussian-forward-rate-field.md) with deterministic volatility, put $F=P(t,U)/P(t,T)$, $K_b=(1+\delta K)^{-1}$, and $v^2=\int_t^T\|\Sigma(s,U)-\Sigma(s,T)\|^2ds$. Under the [T-forward measure](t-forward-measure.md), $F$ is lognormal with that integrated variance. With $d_1=\log(F/K_b)/v+v/2$ and $d_2=d_1-v$, the displayed expression is the [caplet](caplet.md) price. At $v=0$ use the discounted intrinsic bond-put value. Gaussian instantaneous rates do not make the reset floating rate Gaussian; the exponential bond relation is what yields this bond-option formula.

## ↑ Ancestors (9)

1. [Caplet](caplet.md)
2. [Interest-rate cap](interest-rate-cap.md)
3. [Interest rate](interest-rate.md)
4. [Fixed-income security](fixed-income-security.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/iii/solution.md)
