<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Itô formula](../../../../../../ito-s-lemma.md) applied to $F(t,x)=e^{t/2}\cos x$ gives exact cancellation of the [drift](../../../../../../drift-coefficient.md):

$$
d(e^{t/2}\cos B_t)=-e^{t/2}\sin B_t\,dB_t.
$$

On every finite interval $[0,T]$, the [Itô integral](../../../../../../ito-integral.md) is [square-integrable](../../../../../../square-integrable-function.md) since $\mathbb E\int_0^Te^s\sin^2B_s\,ds\leq e^T-1$. Therefore **$e^{t/2}\cos B_t$ is a true [martingale](../../../../../../martingale-split.md), and hence a [local martingale](../../../../../../local-martingale.md).**

For the other [stochastic process](../../../../../../stochastic-process-split.md), $d(B_t-t^2)=dB_t-2t\,dt$. If $B_t-t^2$ were a [local martingale](../../../../../../local-martingale.md), its difference with $B$ would make the continuous [finite-variation process](../../../../../../finite-variation-process.md) $-t^2$ a [local martingale](../../../../../../local-martingale.md), contradicting the fact that a [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md). Also $\mathbb E(B_t-t^2)=-t^2$ is not constant. Thus **$B_t-t^2$ is neither a [local martingale](../../../../../../local-martingale.md) nor a [martingale](../../../../../../martingale-split.md).**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
