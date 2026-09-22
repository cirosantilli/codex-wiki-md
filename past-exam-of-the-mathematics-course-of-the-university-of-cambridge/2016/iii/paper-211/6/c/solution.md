<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The positive [density process](../../../../../../density-process.md) is the [stochastic exponential](../../../../../../doleans-dade-exponential.md)

$$
Z_t=\exp\!\left(\int_0^t a'(S_s)dW_s-\frac12\int_0^t a'(S_s)^2ds\right).
$$

Since $a'$ is bounded, the [Novikov condition](../../../../../../novikov-s-condition.md) holds; $Z$ is a true [martingale](../../../../../../martingale-split.md) with $\mathbb EZ_T=1$ and $Z_T>0$. Thus it defines the stated [equivalent probability measure](../../../../../../equivalent-probability-measure.md). The positive sign in the exponent means that the [Girsanov theorem](../../../../../../girsanov-theorem.md) gives

$$
\widehat W_t=W_t-\int_0^t a'(S_s)ds,
\qquad dS_t=a(S_t)d\widehat W_t+a(S_t)a'(S_t)dt.
$$

Under this [change of measure](../../../../../../change-of-measure.md), applying the [Itô formula](../../../../../../ito-s-lemma.md) to $\pi_t=U(t,S_t)$ produces precisely the [drift](../../../../../../drift-coefficient.md) in its backward equation, which vanishes:

$$
d\pi_t=a(S_t)U_S(t,S_t)d\widehat W_t.
$$

Bounded $a$ and $U_S$ make $\pi$ a true [martingale](../../../../../../martingale-split.md) under $\widehat{\mathbb P}$. Its terminal value is $g'(S_T)$. **Consequently**

$$
\boxed{\pi_t=\mathbb E^{\widehat{\mathbb P}}[g'(S_T)\mid\mathcal F_t].}
$$

The sign can also be checked before changing measure: under the original measure $d\pi=-aa'U_Sdt+aU_SdW$, while the [quadratic covariation](../../../../../../quadratic-covariation.md) term in $d(Z\pi)$ is $Zaa'U_Sdt$, exactly cancelling its [drift](../../../../../../drift-coefficient.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
