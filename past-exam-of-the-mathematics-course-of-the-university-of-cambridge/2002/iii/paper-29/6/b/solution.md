<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the displayed [Gaussian forward-rate covariance drift restriction](../../../../../../gaussian-forward-rate-covariance-drift-restriction.md). Its diagonal instance gives

$$
\mu_{u,u}-\mu_{0,u}=\int_0^u c(w,w,u)\,dw.
$$

Using it on the two parts of the deterministic discounted exponent yields

$$
\begin{aligned}
A(s,T)-A(0,T)
&=\int_0^s\int_0^u c(w,w,u)\,dw\,du
+\int_s^T\int_0^u c(s\wedge w,w,u)\,dw\,du\\
&=\int_0^T\int_0^u c(s\wedge w,w,u)\,dw\,du\\
&=\frac12\int_0^T\int_0^T c(s\wedge u\wedge w,u,w)\,du\,dw
=\frac12v(s,T).
\end{aligned}
$$

The last equality uses [covariance](../../../../../../covariance.md) symmetry to reflect the triangular integration region across its diagonal. The [independent increments](../../../../../../independent-increments.md) of the [integrated Gaussian forward-rate process](../../../../../../integrated-gaussian-forward-rate-process.md) and its conditional [Gaussian moment-generating function](../../../../../../moment-generating-function-of-a-normal-distribution.md) then give, for $r\leq s\leq T$,

$$
\mathbb E[Z_{s,T}\mid\mathcal F_r]
=e^{-A(s,T)-Y(r,T)+(v(s,T)-v(r,T))/2}
=e^{-A(r,T)-Y(r,T)}=Z_{r,T}.
$$

All these prices are [integrable](../../../../../../integrability.md) because their exponents are [Gaussian random variables](../../../../../../gaussian-random-variable.md) with finite [variance](../../../../../../variance-split.md). Thus the mean restriction implies the discounted bond [martingale](../../../../../../martingale-split.md) condition, completing the equivalence of the first two descriptions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
