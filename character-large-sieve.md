# Character large sieve

↑ **Parent:** [Large sieve](large-sieve.md)

For coefficients supported on $N$ consecutive [integers](integer.md),

$$
\sum_{q\leq Q}\frac q{\phi(q)}\sum_{\chi\bmod q}^{*}\left|\sum_na_n\chi(n)\right|^2\leq(Q^2+2\pi N)\sum_n|a_n|^2.
$$

The star restricts to [primitive Dirichlet characters](primitive-dirichlet-character.md). Their [finite Fourier transform of a primitive Dirichlet character](finite-fourier-transform-of-a-primitive-dirichlet-character.md) has normalization of [absolute value](absolute-value.md) $\sqrt q$. [Orthogonality of Dirichlet characters](orthogonality-of-dirichlet-characters.md) therefore bounds the weighted contribution for one modulus by $\sum_{\substack{a\bmod q\\(a,q)=1}}|\sum_na_ne(an/q)|^2$. Sum over $q$ and use the [exponential-sum large sieve](exponential-sum-large-sieve.md) on the distinct [reduced fractions](reduced-fraction.md) of denominators at most $Q$.

## ↑ Ancestors (7)

1. [Large sieve](large-sieve.md)
2. [Sieve theory](sieve-theory.md)
3. [Analytic number theory](analytic-number-theory-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/4/a/solution.md)
