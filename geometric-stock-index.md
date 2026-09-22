# Geometric stock index

↑ **Parent:** [Stock](stock.md)

For positive [stocks](stock.md) satisfying $dS_t^i/S_t^i=\sum_j\sigma_{ij}dW_t^j+\mu_i dt$, let $q=n^{-1}\mathbf1$ and $V=\sigma\sigma^T$. The [Itô formula](ito-s-lemma.md) gives

$$
\log(J_t/J_0)=q^T\sigma W_t+\left(q^T\mu-\frac1{2n}\operatorname{tr}V\right)t.
$$

Thus its volatility is $\sigma^Tq$. This geometric average is generally not the value of the constant equal-weight [self-financing portfolio](self-financing-portfolio.md): its instantaneous drift is $q^T\mu-\operatorname{tr}(V)/(2n)+q^TVq/2$, whereas the fully invested equal-weight portfolio has drift $q^T\mu$.

## ↑ Ancestors (6)

1. [Stock](stock.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Benchmark-relative power-utility portfolio](benchmark-relative-power-utility-portfolio.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40/4/solution.md)
