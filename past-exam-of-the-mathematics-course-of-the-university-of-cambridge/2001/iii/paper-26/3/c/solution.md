<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [bufferless queue output](../../../../../../bufferless-queue-output.md) is

$$
Y^L=\min(S_L,u_L),\qquad u_L=L\lambda+C L^{(1+\beta)/2}.
$$

Put $r_L=L\lambda+B L^{(1+\alpha)/2}$. Since $\alpha<\beta$, we have $r_L<u_L$ for all sufficiently large $L$. Consequently the two [queue overflow](../../../../../../queue-overflow.md) events are exactly equal eventually:

$$
\{Y^L>r_L\}=\{S_L>r_L\}.
$$

Apply the [Poisson moderate deviation principle](../../../../../../poisson-moderate-deviation-principle.md) with exponent $\alpha$ to obtain

$$
\boxed{\lim_L\frac1{L^\alpha}\log\mathbb P(Y^L>r_L)=-\frac{B^2}{2\lambda}.}
$$

There is also an [exponential equivalence](../../../../../../exponential-equivalence.md) proof, which describes the whole output law at this smaller scale. For each $\varepsilon>0$,

$$
\mathbb P\!\left(\frac{|S_L-Y^L|}{L^{(1+\alpha)/2}}>\varepsilon\right)
\le\mathbb P(S_L>u_L).
$$

The right side has strictly negative logarithmic exponent at speed $L^\beta$. Dividing instead by $L^\alpha$ multiplies that negative exponent by $L^{\beta-\alpha}\to\infty$, giving $-\infty$. Thus the centered, scaled input and output are exponentially equivalent and have the same [good rate function](../../../../../../good-rate-function.md). This is the [moderate deviations below a bufferless queue cap](../../../../../../moderate-deviations-below-a-bufferless-queue-cap.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
