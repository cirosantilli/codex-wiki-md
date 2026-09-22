<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any $n\geq0$, take $f_n=T_{n+1}$, the [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) of degree $n+1$. It has $n+2$ alternating extrema of magnitude one on $[-1,1]$. The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) shows that the zero polynomial is best from $\mathcal P_n$, with error one. Since it also lies in $\mathcal P_{n-1}$ when $n\geq1$,

$$
\boxed{E_{n-1}(T_{n+1})=E_n(T_{n+1})=1}.
$$

Now suppose $f^{(n)}(x)\gt0$ throughout $[-1,1]$ and, contrary to the claim, $E_{n-1}(f)=E_n(f)$. A best $p\in\mathcal P_{n-1}$ would then also be best in $\mathcal P_n$. Its error $e=f-p$ would have $n+2$ alternating extrema by the alternation theorem, hence at least $n+1$ distinct zeros. Applying the [Rolle theorem](../../../../../../rolle-theorem.md) $n$ times gives a zero of

$$
e^{(n)}=f^{(n)}-p^{(n)}=f^{(n)},
$$

contradicting positivity. Therefore

$$
\boxed{E_{n-1}(f)\gt E_n(f)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
