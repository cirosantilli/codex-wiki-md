# Exponential sign bracketing

↑ **Parent:** [Exponential search](exponential-search.md)

If $f(0)<0$ and $f(x)>0$ for all sufficiently large positive $x$, testing $1,2,4,\ldots$ eventually finds a positive endpoint. Keep the previous nonpositive endpoint to obtain a bracket. If $t$ is the first successful exponent, there are $t+1$ endpoint tests. Subsequent [sign-bracketing binary search](sign-bracketing-binary-search.md) in the last interval takes $t-1$ tests for $t\geq1$, since its width is $2^{t-1}$. No monotonicity is needed, though intermediate sign crossings may be skipped. Fixed-width [integer overflow](integer-overflow.md) and unreliable floating-point signs require explicit handling; eventual real positivity alone does not guarantee representable machine endpoints.

## ↑ Ancestors (4)

1. [Exponential search](exponential-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
