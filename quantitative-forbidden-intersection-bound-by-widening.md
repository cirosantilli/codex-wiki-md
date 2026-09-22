# Quantitative forbidden-intersection bound by widening

↑ **Parent:** [Forbidden-intersection density increment](forbidden-intersection-density-increment.md)

Let two [set families](set-family.md) on $n$ coordinates forbid cross-intersection size $\ell$, and let $\rho$ be their density product. For $0<\delta\leq1/10$, put $g=\log(1+\delta)$, $h=-\log(1-\delta-2\delta^2)$, and $D=g+h$. Repeated [forbidden-intersection density increments](forbidden-intersection-density-increment.md) terminate when one endpoint of the forbidden interval reaches zero or the remaining dimension. In the first case, if $v$ steps widened the interval, the [cross-intersection bound from cube separation](cross-intersection-bound-from-cube-separation.md) gives $\log\rho\leq-g\ell+Dv-v^2/n\leq-g\ell+D^2n/4$. In the second case, at least $n-\ell$ steps occurred and at most $\ell$ widened, giving $\log\rho\leq-gn+(2g+h)\ell$. For a single [set family](set-family.md) take the square of its density. Choosing $\delta=1/50$ proves $|\mathcal A|\leq1.999^n$ for forbidden intersections $n/4$ and $\lfloor n/8\rfloor$, with small dimensions handled directly.

## ↑ Ancestors (6)

1. [Forbidden-intersection density increment](forbidden-intersection-density-increment.md)
2. [Extremal set theory](extremal-set-theory-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
