<h1 id="17c/solution">Solution</h1>

↑ **Parent:** [17C](../17c.md)

Expanding the order condition about $w=1$ yields $\rho(w)=\sigma_s\sum_{l=1}^s w^{s-l}(w-1)^l/l$ and $\sigma_s=(\sum1/l)^{-1}$. Thus BDF2 has $\rho=w^2-4w/3+1/3$, $\sigma_2=2/3$, and BDF3 has $\rho=w^3-18w^2/11+9w/11-2/11$, $\sigma_3=6/11$. Their first characteristic [polynomials](../../../../../polynomial-split.md) satisfy the root condition, so consistency plus Dahlquist equivalence gives convergence. For BDF2 the stability boundary $z=\rho(e^{i\theta})/(\sigma_2e^{2i\theta})$ has nonnegative real part; hence the whole left half-plane is stable.

## ↑ Ancestors (10)

1. [17C](../17c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
