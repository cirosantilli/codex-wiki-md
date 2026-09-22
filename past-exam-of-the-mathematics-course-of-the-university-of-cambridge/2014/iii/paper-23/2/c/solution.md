<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The constant and first [Fourier coefficients](../../../../../../fourier-coefficient.md) of $\phi^8$ are $1$ and $-16$. In the [weight-four Eisenstein basis at level two](../../../../../../weight-four-eisenstein-basis-at-level-two.md), these force

$$
\boxed{\phi^8=\frac{16E_4(2\tau)-E_4(\tau)}{15}.}
$$

For $n>0$, its $q^n$ coefficient is $-16\sigma_3(n)+256\sigma_3(n/2)$, where the second [divisor sum](../../../../../../divisor-sum.md) is zero if $n$ is odd. The even divisors have cube sum $8\sigma_3(n/2)$, so

$$
\sum_{d\mid n}(-1)^dd^3=16\sigma_3(n/2)-\sigma_3(n).
$$

On the other hand, expanding the eighth power of the [theta series of integer squares](../../../../../../theta-series-of-integer-squares.md) counts ordered integer eight-tuples of square sum $n$. Their sign is $(-1)^{\sum_jm_j}=(-1)^n$, since $m_j^2\equiv m_j\pmod2$. If $r_8(n)$ denotes that count, then

$$
\boxed{\phi^8=\sum_{n\ge0}(-1)^nr_8(n)q^n,\qquad
r_8(n)=16(-1)^n\sum_{d\mid n}(-1)^dd^3\quad(n\ge1).}
$$

Separately **$r_8(0)=1$**, from the all-zero tuple. The positive-divisor formula is not a formula at zero. This is the [eight-square representation formula](../../../../../../eight-square-representation-formula.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
