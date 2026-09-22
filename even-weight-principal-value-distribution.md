# Even-weight principal-value distribution

↑ **Parent:** [Principal-value reciprocal distribution](principal-value-reciprocal-distribution.md)

For a continuous even [function](function-split.md) $f$ on $\mathbb R$, the [Cauchy principal value](cauchy-principal-value.md)

$$
\left\langle\operatorname{pv}\frac{f(x)}x,\phi\right\rangle
=\int_0^\infty f(x)\frac{\phi(x)-\phi(-x)}x\,dx
$$

defines a [distribution](distribution-mathematical-analysis.md) of [order of a distribution](order-of-a-distribution.md) at most one. For [test functions](test-function.md) supported in $[-R,R]$, the absolute value is at most $2R\max_{[0,R]}|f|\,\|\phi'\|_\infty$, since the numerator is bounded by $2x\|\phi'\|_\infty$. When $\phi(0)=0$, the expression equals the absolutely convergent ordinary integral $\int f\phi/x$.

It is a [regular distribution](regular-distribution.md) exactly when $\int_0^r|f(x)|/x\,dx<\infty$ for some $r>0$. Necessity follows by testing away from zero: any representing [locally integrable function](locally-integrable-function.md) must equal $f/x$ [almost everywhere](almost-everywhere.md) off zero. Sufficiency follows from absolute convergence. Continuity with $f(0)=0$ alone does not suffice: $f(x)=1/\log(1/|x|)$ near zero gives the divergent integral $\int_1^\infty ds/s$.

```
Target: L1-normalized dilation of a distribution. Parent: Dilation of a distribution. Intended file: distribution-theory.bigb.
```

## ↑ Ancestors (7)

1. [Principal-value reciprocal distribution](principal-value-reciprocal-distribution.md)
2. [Multiplication of a distribution by a smooth function](multiplication-of-a-distribution-by-a-smooth-function.md)
3. [Distribution theory](distribution-theory-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/1/b/i/solution.md)
- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/1/b/ii/solution.md)
