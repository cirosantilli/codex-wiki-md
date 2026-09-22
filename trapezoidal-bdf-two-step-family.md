# Trapezoidal-BDF two-step family

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

This real-parameter [linear multistep method](linear-multistep-method.md) has formal order two except at the degenerate value $\alpha=2$, where its local symbol vanishes to fourth degree. The zero-stability roots are $1$ and $\alpha-1$, so it is convergent exactly for $0\leq\alpha<2$. Every convergent member is [A-stable](a-stability.md): the [boundary-locus test for multistep A-stability](boundary-locus-test-for-multistep-a-stability.md) gives nonnegative real part $\alpha(2-\alpha)(1-\cos\theta)^2/(2|\sigma(e^{i\theta})|^2)$, with no unit-circle denominator zero for $0<\alpha<2$. At $\alpha=0$ the two interlaced sequences obey a trapezoidal step of length $2h$. At $\alpha=4/3$ it is the [BDF2 method](second-order-backward-differentiation-formula.md). The endpoint two fails the [root condition for a multistep method](root-condition-for-a-multistep-method.md) even though canceling a common polynomial factor resembles the [trapezoidal rule](trapezoidal-rule.md).

## ↑ Ancestors (6)

1. [Linear multistep method](linear-multistep-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Second-order backward differentiation formula](second-order-backward-differentiation-formula.md)
