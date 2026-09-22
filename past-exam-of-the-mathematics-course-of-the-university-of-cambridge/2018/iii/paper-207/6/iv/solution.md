<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The minimum exceeds $t$ exactly when both times exceed $t$. By [independence](../../../../../../independent-random-variables.md),

$$
\mathbb P(X>t)=F_A(t)F_B(t).
$$

Differentiating its [survivor function](../../../../../../survival-function.md) gives

$$
\boxed{f_X(t)=-\frac{d}{dt}[F_A(t)F_B(t)]
=f_A(t)F_B(t)+F_A(t)f_B(t).}
$$

The [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md) then gives

$$
\boxed{\mathbb E X=\int_0^\infty F_A(t)F_B(t)\,dt.}
$$

Equivalently, [integration by parts](../../../../../../integration-by-parts.md) in $\int_0^R t f_X(t)\,dt$ gives $-RF_A(R)F_B(R)+\int_0^R F_A(t)F_B(t)\,dt$. The assumed $tF_B(t)\to0$ makes the boundary term vanish, since $0\leq F_A\leq1$.

The stated tail condition does not itself guarantee a finite mean. For example, the proper [survivor functions](../../../../../../survival-function.md)

$$
F_B(t)=\frac1{(1+t)\log(e+t)},\qquad
F_A(t)=\frac1{\log(e+\log(1+t))}
$$

satisfy $tF_B(t)\to0$, but their product behaves as $1/[t\log t\log\log t]$, whose integral diverges. Thus the displayed expectation is valid as an extended nonnegative value; finiteness needs integrability of the product. The [exponential distribution](../../../../../../exponential-distribution.md) in the next part guarantees that finiteness.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
