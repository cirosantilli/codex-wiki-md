<h1 id="29k/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Under $\mathbb Q$,

$$
\log S_T\sim N\left(\log S_0+(r-\tfrac12\sigma^2)T,\sigma^2T\right).
$$

Define

$$
d_+=\frac{\log(S_0/K)+(r+\tfrac12\sigma^2)T}{\sigma\sqrt T},
\qquad
d_-=d_+-\sigma\sqrt T
=\frac{\log(S_0/K)+(r-\tfrac12\sigma^2)T}{\sigma\sqrt T}.
$$

The [standard normal cumulative distribution function](../../../../../../standard-normal-distribution-function.md) $\Phi$ then gives

$$
\mathbb Q(S_T>K)=\Phi(d_-),
\qquad
\mathbb E_{\mathbb Q}[S_T\mathbf1_{\{S_T>K\}}]=S_0e^{rT}\Phi(d_+).
$$

Substitution into the discounted expected payoff yields the [Black-Scholes formula](../../../../../../black-scholes-formula.md)

$$
\boxed{V_0=S_0\Phi(d_+)-e^{-rT}K\Phi(d_-)}.
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
