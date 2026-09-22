<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\tau=T-t$. In the [Black-Scholes formula](../../../../../black-scholes-formula.md), both $d_1$ and $d_2$ depend on $x,K$ only through $\log(x/K)$. Replacing them by $\lambda x,\lambda K$ leaves that ratio unchanged. Each prefactor in the put formula acquires the same factor $\lambda$, giving

$$
p(t,\lambda x;\lambda K,T)
=\lambda Ke^{-r\tau}\Phi(-d_2)-\lambda x\Phi(-d_1)
=\boxed{\lambda p(t,x;K,T).}
$$

This is degree-one [homogeneity](../../../../../homogeneity.md) of the [European put option](../../../../../european-put-option.md) price in its spot and strike together.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
