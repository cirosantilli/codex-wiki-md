<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $F(s)=-\zeta'(s)/\zeta(s)$ and $\psi_\Gamma=\Gamma'/\Gamma$. The [global partial-fraction expansion of the zeta logarithmic derivative](../../../../../global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative.md) is

$$
F(s)=\frac1{s-1}-\frac12\log\pi+\frac12\psi_\Gamma(1+s/2)-B-\sum_\rho\left(\frac1{s-\rho}+\frac1\rho\right),\qquad B=\log2+\frac12\log\pi-1-\frac\gamma2.
$$

Here $\gamma$ is the [Euler--Mascheroni constant](../../../../../euler-s-constant.md), and the sum includes multiplicities of the [Nontrivial zeros of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md). The paired terms are locally absolutely convergent away from their [poles](../../../../../pole.md), by the [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md). This identity follows by differentiating the genus-one [Hadamard factorization](../../../../../hadamard-factorization-theorem.md) of the [Riemann xi function](../../../../../riemann-xi-function.md) and using the [Gamma function recurrence](../../../../../gamma-function-recurrence.md).

We first prove the classical [zero-free region of the Riemann zeta function](../../../../../zero-free-region-of-the-riemann-zeta-function.md). The [Euler-product nonvanishing of the Riemann zeta function](../../../../../euler-product-nonvanishing-of-the-riemann-zeta-function.md) and its [functional equation](../../../../../functional-equation.md) place every nontrivial zero in the closed strip $0\le\beta\le1$; no assertion about zeros on its boundary is needed yet. The [real logarithmic derivative of Riemann xi](../../../../../real-logarithmic-derivative-of-riemann-xi.md) and the [digamma function](../../../../../digamma-function.md) asymptotic imply, for $1<\sigma\le2$ and $|t|\ge1$,

$$
\Re F(\sigma+it)\le C\log(|t|+2)-\sum_\rho\frac{\sigma-\beta}{(\sigma-\beta)^2+(t-\gamma_\rho)^2}.
$$

Every summand being subtracted is nonnegative. If $\beta+it$ is a zero, retaining its summand gives $\Re F(\sigma+it)\le C\log(|t|+2)-1/(\sigma-\beta)$; at height $2t$ the upper bound $C\log(|t|+2)$ suffices. At real $\sigma$ the simple [pole](../../../../../pole.md) of $\zeta$ gives $F(\sigma)=1/(\sigma-1)+O(1)$.

For $\sigma>1$, the [Dirichlet series](../../../../../dirichlet-series.md) $F(s)=\sum_n\Lambda(n)n^{-s}$ has nonnegative coefficients. The identity $3+4\cos u+\cos2u=2(1+\cos u)^2\ge0$ therefore gives the [three-four-one zero-free-region argument](../../../../../three-four-one-zero-free-region-argument.md)

$$
0\le3F(\sigma)+4\Re F(\sigma+it)+\Re F(\sigma+2it).
$$

With $L=\log(|t|+2)$, a zero at $\beta+it$ would consequently satisfy

$$
\frac4{\sigma-\beta}\le\frac3{\sigma-1}+CL.
$$

Choose $\sigma=1+a/L$, with an absolute $a>0$ sufficiently small, and put $c=a/8$. If $\beta\ge1-c/L$, this inequality would imply $4/(a+c)\le3/a+C$. But $4/(a+a/8)-3/a=5/(9a)>C$ for small enough $a$, a contradiction.

For any fixed $t\ne0$, the same positivity inequality as $\sigma\downarrow1$ excludes a zero at $1+it$: its negative contribution has coefficient at least four, whereas the real [pole](../../../../../pole.md) contributes only three. Any zero at $1+2it$ only strengthens the contradiction. The [pole](../../../../../pole.md) at $s=1$ has a zero-free punctured neighbourhood. By compactness, the remaining bounded-height portion of the line has a zero-free neighbourhood as well. Shrink $c$ to combine these facts with the large-height bound. Hence

$$
\boxed{\zeta(\beta+i\gamma)\ne0\quad\text{if}\quad\beta\ge1-\frac c{\log(|\gamma|+2)},}
$$

with the understanding that $s=1$ is a [pole](../../../../../pole.md).

The [Riemann–von Mangoldt explicit formula](../../../../../riemann-von-mangoldt-explicit-formula.md) for the [Second Chebyshev function](../../../../../second-chebyshev-function.md), with half weight at a prime-power endpoint, is

$$
\psi_0(x)=x-\lim_{T\to\infty}\sum_{|\Im\rho|\le T}\frac{x^\rho}{\rho}-\log(2\pi)-\frac12\log(1-x^{-2}),\qquad x>1.
$$

The zero sum uses symmetric height truncation. To estimate it, take a half-integer $x$ and use the [truncated explicit formula for the second Chebyshev function](../../../../../truncated-explicit-formula-for-the-second-chebyshev-function.md)

$$
\psi(x)=x-\sum_{|\Im\rho|\le T}\frac{x^\rho}{\rho}+O\left(\frac{x\log^2(xT)}T+\log x\right),\qquad 2\le T\le x.
$$

The zero-free region gives $|x^\rho|\le x\exp(-c\log x/\log(T+2))$ for these zeros. The [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md) and [partial summation](../../../../../abel-s-summation-formula.md) give $\sum_{|\Im\rho|\le T}|\rho|^{-1}\ll\log^2(T+2)$. Choose $T=\exp(\sqrt{\log x})$. Both the zero sum and the truncation error are then $O(xe^{-c'\sqrt{\log x}})$ after reducing the positive constant to absorb logarithmic factors. Replacing an arbitrary $X$ by $\lfloor X\rfloor+1/2$ preserves the [Von Mangoldt function](../../../../../von-mangoldt-function.md) sum and changes the main term by at most one. This proves the requested form of the [Prime number theorem](../../../../../prime-number-theorem.md):

$$
\boxed{\sum_{n\le X}\Lambda(n)=X+O\left(Xe^{-c'\sqrt{\log X}}\right).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
