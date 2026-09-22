<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $r>0$, write $m_r=v_dr^d$, $a_r=\int_{B(0,r)}e^{-f(x)}\,dx$, and $L=\mathbb Ee^{-M(f)}$. The [count-weighted Laplace functional of a Poisson random measure](../../../../../../../count-weighted-laplace-functional-of-a-poisson-random-measure.md) and the [Poisson distribution](../../../../../../../poisson-distribution.md) give

$$
\frac{\mathbb E[N_re^{-M(f)}]}{\mathbb P(N_r\geq1)}=L\frac{a_r}{1-e^{-m_r}}.
$$

To compute the other numerator, on $\{N_r=0\}$ the inside contribution to $M(f)$ vanishes. The restrictions of the [Poisson random measure](../../../../../../../poisson-random-measure.md) to the ball and its complement are independent; this follows first for their simple-function integrals from independent counts, then by approximation. Hence

$$
\begin{aligned}
\mathbb E[e^{-M(f)}\mathbf1_{\{N_r=0\}}]
&=e^{-m_r}\exp\left(-\int_{B(0,r)^c}(1-e^{-f(x)})\,dx\right)\\
&=L e^{-a_r}.
\end{aligned}
$$

Subtract from $L$ and divide by $\mathbb P(N_r\geq1)$ to find

$$
\mathbb E[e^{-M(f)}\mid N_r\geq1]=L\frac{1-e^{-a_r}}{1-e^{-m_r}}.
$$

Continuity of $f$ at zero gives

$$
\left|\frac{a_r}{m_r}-e^{-f(0)}\right|\leq\sup_{|x|<r}|e^{-f(x)}-e^{-f(0)}|\longrightarrow0.
$$

Also $(1-e^{-z})/z\to1$ as $z\downarrow0$. Applying these facts to the two exact expressions proves the [small-ball conditioning for a Poisson random measure](../../../../../../../small-ball-conditioning-for-a-poisson-random-measure.md):

$$
\boxed{\lim_{r\downarrow0}\mathbb E[e^{-M(f)}\mid N_r\geq1]
=\lim_{r\downarrow0}\frac{\mathbb E[N_re^{-M(f)}]}{\mathbb P(N_r\geq1)}
=\exp\left(-f(0)-\int_{\mathbb R^d}(1-e^{-f(x)})\,dx\right).}
$$

One can also see equality of the limits without the exact first formula: since $0\leq e^{-M(f)}\leq1$, the difference of the two quantities lies between zero and $[m_r-(1-e^{-m_r})]/(1-e^{-m_r})\to0$. The conditioning is used only at positive $r$, where its event has positive probability; it is not conditioning directly on a point at the origin.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
