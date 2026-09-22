<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the backward equation for $V$ with respect to the [stock](../../../../../../stock.md) state, and put $w=V_S$. The product derivative of $a^2/2$ is $aa'$, giving

$$
w_t+aa'w_S+\frac12a^2w_{SS}=0,\qquad w(T,S)=g'(S).
$$

The assumed smoothness and bounded derivatives put $w$ in the uniqueness class for the equation defining $U$. Therefore $U=V_S$, and $\pi_t=V_S(t,S_t)$ is the [option delta](../../../../../../option-delta.md). Substituting in the [Itô integral](../../../../../../ito-integral.md) from part (a) and using $dS_t=a(S_t)dW_t$ gives **the self-financing representation**

$$
\boxed{\xi_t=V(0,S_0)+\int_0^t\pi_s\,dS_s,\qquad\pi_t=V_S(t,S_t).}
$$

The boundedness hypotheses justify both [stochastic integrals](../../../../../../stochastic-integral.md). This derivation does not divide by $a$ and remains valid even at states with zero [diffusion amplitude](../../../../../../diffusion-amplitude.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
