# Reed-Solomon key equation

↑ **Parent:** [Primitive cyclic Reed-Solomon code](primitive-cyclic-reed-solomon-code.md)

With [syndromes](syndrome.md) $S_\ell=\sum_i E_i X_i^{b+\ell}$ and distinct error-location values $X_i$, form $S(z)=\sum_{\ell=0}^{n-k-1}S_\ell z^\ell$ and the [error locator polynomial](error-locator-polynomial.md) $\Lambda(z)=\prod_i(1-X_i z)$. There is an [error evaluator polynomial](error-evaluator-polynomial.md) $\Omega$ of degree less than the number of errors satisfying the key equation. When the number of errors is at most $\lfloor(n-k)/2\rfloor$, the [Berlekamp-Massey algorithm](berlekamp-massey-algorithm.md) or [extended Euclidean algorithm](extended-euclidean-algorithm.md) recovers these polynomials, normalized by $\Lambda(0)=1$.

## ↑ Ancestors (8)

1. [Primitive cyclic Reed-Solomon code](primitive-cyclic-reed-solomon-code.md)
2. [Reed-Solomon error correction](reed-solomon-error-correction.md)
3. [Linear code](linear-code.md)
4. [Coding theory](coding-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Error evaluator polynomial](error-evaluator-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-87/3/solution.md)
