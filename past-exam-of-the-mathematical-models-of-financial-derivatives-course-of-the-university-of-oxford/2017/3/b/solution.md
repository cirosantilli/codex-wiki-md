<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [perpetual American call option](../../../../perpetual-american-call-option.md), substitute a power $S^q$ into the stationary [Black-Scholes equation with continuous stock dividends](../../../../black-scholes-equation-with-continuous-stock-dividends.md). The [characteristic equation](../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is

$$
F(q)=\tfrac12\sigma^2q(q-1)+(r-y)q-r=0.
$$

Its two [roots](../../../../root-of-a-root-system.md) have negative product $-2r/\sigma^2$, so one is negative and one positive. The condition at zero excludes the negative power. Since $F(1)=-y<0$ and $F(q)\to\infty$ as $q\to\infty$, the positive root satisfies $p>1$; explicitly,

$$
p=\frac{-(r-y-\sigma^2/2)+\sqrt{(r-y-\sigma^2/2)^2+2r\sigma^2}}{\sigma^2}.
$$

Value matching gives $C(S)=(\hat S-K)(S/\hat S)^p$. The [smooth fit](../../../../smooth-pasting.md) condition gives $p(\hat S-K)/\hat S=1$, hence

$$
\boxed{\hat S=\frac{pK}{p-1},\qquad
C(S)=\begin{cases}(\hat S-K)(S/\hat S)^p,&0\leq S<\hat S,\\S-K,&S\geq\hat S.\end{cases}}
$$

As $y\downarrow0$, the positive root tends to $1$ from above, so $\boxed{p\to1,\ \hat S\to\infty}$. For fixed $S$, the value tends to $S$. In the dividend-free perpetual limit no finite threshold attains that supremum; this agrees with the finite-maturity [no early exercise of a call without dividends](../../../../no-early-exercise-of-a-call-without-dividends.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
