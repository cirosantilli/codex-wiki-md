# Squaring recurrence under integer halving

↑ **Parent:** [Recurrence relation](recurrence-relation.md)

For $T(n)=1$ at $n\leq3$ and $T(n)=2T(\lfloor n/2\rfloor)^2$ otherwise, put $d=\max(0,\lfloor\log_2n\rfloor-1)$ for [positive integer](positive-integer.md) $n$. Taking [logarithms](logarithm.md) gives $S(n)=1+2S(\lfloor n/2\rfloor)$, hence $S(n)=2^d-1$ and $T(n)=2^{2^d-1}$. These constant-value plateaux have exponential envelopes $2^{\Theta(n)}$, but do not justify $\Theta(2^{n/2})$ for all [integer](integer-split.md) inputs.

## ↑ Ancestors (8)

1. [Recurrence relation](recurrence-relation.md)
2. [Sequence](sequence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
