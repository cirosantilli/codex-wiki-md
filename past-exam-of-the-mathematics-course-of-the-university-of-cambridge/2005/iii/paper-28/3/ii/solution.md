<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The permitted zero-count bound $N(T)\ll T\log(T+2)$ implies, by [partial summation](../../../../../../abel-s-summation-formula.md),

$$
\sum_{|\rho|<T}\frac1{|\rho|}\ll\log^2(T+2).
$$

Indeed, the zeros with $|\rho|\leq1$ contribute a bounded amount since $\xi(0)\ne0$; the rest contribute $N(T)/T+\int_1^TN(u)u^{-2}\,du$. For every zero in the sum, the preceding [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md) gives

$$
x^\beta\leq x\exp\left(-\frac{c\log x}{\log(T+2)}\right).
$$

The supplied [truncated explicit formula for the second Chebyshev function](../../../../../../truncated-explicit-formula-for-the-second-chebyshev-function.md) therefore implies

$$
|\psi(x)-x|\ll
x\exp\left(-\frac{c\log x}{\log(T+2)}\right)\log^2(T+2)
+\frac{x\log^2x}{T}.
$$

Choose $T=\exp(a\sqrt{\log x})$, with any fixed positive $a$ and then, for example, $a=\sqrt c$. Both terms have exponential decay in $\sqrt{\log x}$, and the logarithmic factors can be absorbed by slightly decreasing its coefficient. Hence, for some absolute $b>0$,

$$
\boxed{\psi(x)=x+O\bigl(xe^{-b\sqrt{\log x}}\bigr),\qquad \psi(x)\sim x.}
$$

If the truncated formula is taken only at admissible heights and non-prime-power endpoints, choose such heights of the same size and first apply it at half-integers. Monotonicity and the $O(\log x)$ jump of $\psi$ at an [integer](../../../../../../integer.md) transfer this bound to all $x$; these convention choices do not change the conclusion.

To pass from [prime powers](../../../../../../prime-power.md) to [primes](../../../../../../prime-number.md), let $\vartheta(x)=\sum_{p\leq x}\log p$. The higher prime-power contribution satisfies

$$
0\leq\psi(x)-\vartheta(x)
=\sum_{k\geq2}\sum_{p\leq x^{1/k}}\log p
\ll\sqrt x\log^2x=o(x).
$$

Thus $\vartheta(x)\sim x$. Apply [partial summation](../../../../../../abel-s-summation-formula.md) again:

$$
\pi(x)=\frac{\vartheta(x)}{\log x}
+\int_2^x\frac{\vartheta(t)}{t\log^2t}\,dt.
$$

The integral is $O(x/\log^2x)$: use $\vartheta(t)\ll t$ and split at $\sqrt x$. It is therefore smaller than the first term, which is asymptotic to $x/\log x$. This proves the [Prime number theorem](../../../../../../prime-number-theorem.md) in the requested form

$$
\boxed{\pi(x)\sim\frac{x}{\log x}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
