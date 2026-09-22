<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We derive the required [Calderón–Zygmund decomposition](../../../../../../calderon-zygmund-decomposition.md) and apply the preceding two parts. Use the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$, and put $A=\|\widehat K\|_\infty$. The [Plancherel theorem](../../../../../../plancherel-theorem.md) gives

$$
\|Tf\|_2\leq A\|f\|_2.
$$

For completeness this starts with smooth rapidly decreasing inputs, where $\widehat{K*f}=\widehat K\widehat f$, and extends by $L^2$ density. It agrees with the pointwise [convolution](../../../../../../convolution.md) in the question: if $f_j\to f$ in $L^2$, then $\|K*(f_j-f)\|_\infty\leq\|K\|_2\|f_j-f\|_2$. Thus there is no need to assume that $K$ itself is integrable.

Fix $f\in L^1(\mathbb R^d)$, let $F=\|f\|_1$, and choose $\lambda>0$. Select the maximal dyadic [cubes](../../../../../../cube.md) $Q$ for which $|Q|^{-1}\int_Q|f|>\lambda$. They exist above every qualifying [cube](../../../../../../cube.md) because averages over increasingly large ancestors tend to zero. They are disjoint, their total volume is at most $F/\lambda$, and maximality gives

$$
\lambda<\frac1{|Q|}\int_Q|f|\leq2^d\lambda.
$$

Outside their union, dyadic differentiation gives $|f|\leq\lambda$ almost everywhere. One can obtain this differentiation fact from the allowed [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md): on each fixed dyadic [cube](../../../../../../cube.md) the averages are [conditional expectations](../../../../../../conditional-expectation.md) of the integrable restriction, their almost-everywhere limit exists, and approximation by dyadic step functions shows in $L^1$ that this limit is $f$.

Let $f_Q=|Q|^{-1}\int_Qf$, define $g=f$ outside the selected [cubes](../../../../../../cube.md) and $g=f_Q$ on $Q$, and set $b_Q=(f-f_Q)\mathbf1_Q$. This constructs

$$
f=g+b,\qquad b=\sum_Qb_Q,\qquad \int b_Q=0,
$$

with the estimates

$$
\|g\|_\infty\leq2^d\lambda,\qquad \|g\|_1\leq F,\qquad
\|g\|_2^2\leq2^d\lambda F,\qquad \sum_Q\|b_Q\|_1\leq2F.
$$

These follow by integrating separately on each selected [cube](../../../../../../cube.md); $|f_Q||Q|\leq\int_Q|f|$ gives both the good-part [norm](../../../../../../norm.md) bound and the last cancellation-error bound.

Let $\Omega=\bigcup_Q\widehat Q$, with the dilation $L=4\sqrt d$ from part (ii). Then $|\Omega|\leq L^dF/\lambda$. On its complement, part (i), followed by part (ii), gives

$$
\int_{\Omega^c}|Tb|\leq\sum_Q\int_{\Omega^c}|Tb_Q|
\leq\sum_Q\int_{\widehat Q^c}|Tb_Q|\leq2CF.
$$

Finally, $|Tf|>\lambda$ implies $|Tg|>\lambda/2$ or $|Tb|>\lambda/2$. The first alternative is controlled by the $L^2$ operator bound, and the second by the last integral outside $\Omega$. Hence

$$
\begin{aligned}
|\{|Tf|>\lambda\}|
&\leq|\Omega|+\frac{4}{\lambda^2}\|Tg\|_2^2
+\frac{2}{\lambda}\int_{\Omega^c}|Tb|\\
&\leq\left(L^d+2^{d+2}A^2+4C\right)\frac{F}{\lambda}.
\end{aligned}
$$

Thus **$T$ has weak type $(1,1)$**, with a constant depending only on the dimension, the bounded [Fourier transform](../../../../../../fourier-transform.md), and the [Hörmander integral kernel condition](../../../../../../hormander-integral-kernel-condition.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
