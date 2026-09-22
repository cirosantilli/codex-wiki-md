<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

The [Lebesgue differentiation theorem](../../../../../lebesgue-differentiation-theorem.md) states that if $f\in L^1_{\mathrm{loc}}(\mathbb R^n)$, then

$$
\lim_{r\downarrow0}\frac1{\lambda(B_r(x))}\int_{B_r(x)}f(y)\,d\lambda(y)=f(x)
$$

for [Lebesgue almost every](../../../../../almost-everywhere.md) $x$. The [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md) states that if two sigma-finite measures satisfy $\nu\ll\mu$, then there is a nonnegative measurable function $h=d\nu/d\mu$, unique $\mu$-almost everywhere, such that $\nu(E)=\int_Eh\,d\mu$.

For any $t\in[0,1]$, take $z=0$ and let $B$ be a planar sector of angle $2\pi t$. Every disc centred at the origin meets this sector in the proportion

$$
\frac{\lambda(B\cap B_r(0))}{\lambda(B_r(0))}=t,
$$

so its [measure density](../../../../../measure-density.md) at $0$ is $t$.

Apply the differentiation theorem to the [indicator function](../../../../../indicator-function.md) $1_A$. Its averages over balls are exactly $\rho_{\lambda,A}(x)$, so the [Lebesgue density theorem](../../../../../lebesgue-s-density-theorem.md) gives

$$
\rho_{\lambda,A}(x)=1_A(x)\in\{0,1\}
$$

almost everywhere. If $\lambda(A)=0$, every numerator vanishes, so the density is zero wherever its denominator is nonzero. Conversely, if the density vanishes almost everywhere, the displayed identity gives $1_A=0$ almost everywhere, hence $\lambda(A)=0$.

Finally suppose $\nu$ and $\lambda$ are [mutually absolutely continuous measures](../../../../../mutually-absolutely-continuous-measures.md). Write $d\nu=h\,d\lambda$. Then $0<h(x)<\infty$ almost everywhere by the [positive Radon-Nikodym derivative](../../../../../positive-radon-nikodym-derivative.md) result. At almost every $x$, the differentiation theorem applied to both $h$ and $h1_A$ gives

$$
\rho_{\nu,A}(x)
=\lim_{r\downarrow0}
\frac{\int_{B_r(x)}h1_A\,d\lambda}{\int_{B_r(x)}h\,d\lambda}
=\frac{h(x)1_A(x)}{h(x)}=1_A(x).
$$

**Thus the $\nu$-density also exists and belongs to $\{0,1\}$ at $\lambda$-almost every point.**

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
