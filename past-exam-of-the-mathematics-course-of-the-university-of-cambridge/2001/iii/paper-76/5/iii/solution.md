<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Normalize the selected derivative correlations by

$$
c_k=\frac1N\widehat{\Delta_kf}(\phi(k))=\mathbb E_x f(x+k)\overline{f(x)}e(-\phi(k)x/N).
$$

They satisfy $|c_k|\le1$, and the hypothesis gives $\sum_{k\in B}|c_k|^2\ge\alpha N$. Thus $T=\sum_{k\in B}|c_k|\ge\alpha N$. Choose phases $\omega_k$ of modulus one so that $\omega_kc_k=|c_k|$, with any choice if $c_k=0$. Then

$$
T=\mathbb E_x\overline{f(x)}\sum_{k\in B}\omega_kf(x+k)e(-\phi(k)x/N).
$$

One [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) gives

$$
T^2\le\mathbb E_x\left|\sum_{k\in B}\omega_kf(x+k)e(-\phi(k)x/N)\right|^2.
$$

Expand into pairs $a,b\in B$ and group them by $t=a-b$, $r=\phi(a)-\phi(b)$. After translating $y=x+b$, the derivative correlation is

$$
C(t,r)=\mathbb E_y f(y+t)\overline{f(y)}e(-ry/N).
$$

The grouped coefficient is

$$
\gamma(t,r)=\sum_{\substack{a,b\in B\\a-b=t\\\phi(a)-\phi(b)=r}}
\omega_a\overline{\omega_b}\,e(rb/N).
$$

Consequently $T^2\le\sum_{t,r}\gamma(t,r)C(t,r)$, whose right-hand side is the real nonnegative expanded square. A second [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) yields

$$
T^4\le\left(\sum_{t,r}|\gamma(t,r)|^2\right)\left(\sum_{t,r}|C(t,r)|^2\right).
$$

If $m(t,r)$ counts the pairs in the displayed coefficient, then $|\gamma(t,r)|\le m(t,r)$. Thus $\sum|\gamma|^2\le\sum m^2=E(\Gamma)$, the [additive energy of a frequency graph](../../../../../../additive-energy-of-a-frequency-graph.md) $\Gamma=\{(k,\phi(k)):k\in B\}$. Equality of two pair differences is equivalent, by permuting the four labels, to equality of the two requested sums in each coordinate.

For every $t$, [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) in normalized Fourier convention gives

$$
\sum_r|C(t,r)|^2=\mathbb E_y|f(y+t)|^2|f(y)|^2\le1.
$$

There are $N$ shifts, so $T^4\le NE(\Gamma)$. Since $T\ge\alpha N$, we conclude

$$
\boxed{E(\Gamma)\ge\alpha^4N^3.}
$$

This is precisely the number of ordered $(a,b,c,d)\in B^4$ satisfying both $a+b=c+d$ and $\phi(a)+\phi(b)=\phi(c)+\phi(d)$, all modulo $N$. It proves [squared derivative correlations force frequency-graph energy](../../../../../../squared-derivative-correlations-force-frequency-graph-energy.md) with the constant and exact equalities stated, rather than approximate frequency matching.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
