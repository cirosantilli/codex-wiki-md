# Selberg sieve denominator asymptotic

↑ **Parent:** [Selberg sieve weights](selberg-sieve-weights.md)

Put $g(n)=\mu(n)^2/\varphi(n)$. As a [Dirichlet convolution](dirichlet-convolution.md), $g=h*(n\mapsto1/n)$, where $h$ is a [multiplicative arithmetic function](multiplicative-function.md) with $h(p)=1/(p(p-1))$, $h(p^2)=-1/(p(p-1))$, and $h(p^j)=0$ for $j\ge3$. The local sums are one, so $\sum_nh(n)=1$. The series $\sum_n|h(n)|\log(2n)$ converges, since the prime-local errors are $O((\log p)/p^2)$. Consequently $G(z)=\sum_{d\le z}h(d)H_{\lfloor z/d\rfloor}=\log z+O(1)$ by the [harmonic number](harmonic-number.md) estimate $H_m=\log m+O(1)$. This identifies the leading constant in the one-dimensional [Selberg upper-bound sieve](selberg-upper-bound-sieve.md).

## ↑ Ancestors (10)

1. [Selberg sieve weights](selberg-sieve-weights.md)
2. [Selberg upper-bound sieve](selberg-upper-bound-sieve.md)
3. [Selberg sieve](selberg-sieve.md)
4. [Upper-bound sieve](upper-bound-sieve.md)
5. [Sieve theory](sieve-theory.md)
6. [Analytic number theory](analytic-number-theory-split.md)
7. [Number theory](number-theory-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/4/solution.md)
- [Uniform interval bound from optimal Selberg weights](uniform-interval-bound-from-optimal-selberg-weights.md)
