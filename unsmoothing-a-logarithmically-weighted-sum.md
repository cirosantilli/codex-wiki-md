# Unsmoothing a logarithmically weighted sum

↑ **Parent:** [Logarithmically smoothed Perron formula](logarithmically-smoothed-perron-formula.md)

Suppose $|a_n|\le(\log(2n))^k$ and $A(x)=\sum_{n\le x}a_n\log(x/n)=O(x(\log x)^\beta)$, with $0\le\beta\le k$. For $0<h\le1$, direct subtraction gives

$$
A(xe^h)-A(x)=h\sum_{n\le x}a_n+\sum_{x<n\le xe^h}a_n\log(xe^h/n).
$$

The last term has absolute value $O((xh^2+h)(\log x)^k)$. Choose $h=(\log x)^{(\beta-k)/2}$ to obtain the displayed bound, with an additional $O((\log x)^k)$ term harmless as $x\to\infty$ for fixed $k$. This elementary finite-difference argument converts a [logarithmically smoothed Perron formula](logarithmically-smoothed-perron-formula.md) bound to cancellation in its original [partial sum](partial-sum.md).

## ↑ Ancestors (8)

1. [Logarithmically smoothed Perron formula](logarithmically-smoothed-perron-formula.md)
2. [Perron's formula](perron-s-formula.md)
3. [Dirichlet series](dirichlet-series.md)
4. [Analytic number theory](analytic-number-theory-split.md)
5. [Number theory](number-theory-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/2/solution.md)
