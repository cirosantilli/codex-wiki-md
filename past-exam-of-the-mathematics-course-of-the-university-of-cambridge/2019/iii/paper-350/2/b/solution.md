<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A simple choice is an independent [Laplace distribution](../../../../../../laplace-distribution.md) at each pixel, giving a [Laplace prior for sparse images](../../../../../../laplace-prior-for-sparse-images.md):

$$
\boxed{\pi_0(u)=\left(\frac\lambda2\right)^d
\exp\left(-\lambda\sum_{j=1}^d|u_j|\right),\qquad\lambda>0.}
$$

Its negative log density penalizes the [L1 norm](../../../../../../l1-norm.md). Relative to a [normal distribution](../../../../../../normal-distribution.md), it combines a sharp peak at zero with heavier tails, allowing most pixels to lie near the background level while a few have appreciable intensity. Quantitatively, $\mathbb P(|u_j|>\tau)=e^{-\lambda\tau}$, so the expected number of appreciable pixels is $de^{-\lambda\tau}$. Choosing $\lambda\tau$ large makes this small. This is a simple sparsity model: it does not enforce that nearby active pixels form connected objects, nor does its continuous density give exact zero pixels positive probability. Additional spatial modelling would be needed to insist on contiguous shapes.

To sample, draw independent $U_j\sim\mathcal U(0,1)$ and use [inverse transform sampling](../../../../../../inverse-transform-sampling.md):

$$
\boxed{u_j=\begin{cases}
\lambda^{-1}\log(2U_j),&0<U_j\leq\tfrac12,\\
-\lambda^{-1}\log(2(1-U_j)),&\tfrac12<U_j<1.
\end{cases}}
$$

The endpoint events have probability zero and can be assigned arbitrary finite values. To justify the rule, the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of a centered [Laplace distribution](../../../../../../laplace-distribution.md) is

$$
F(x)=\begin{cases}
\tfrac12e^{\lambda x},&x\leq0,\\
1-\tfrac12e^{-\lambda x},&x\geq0.
\end{cases}
$$

The displayed rule is $F^{-1}(U_j)$, so $\mathbb P(u_j\leq x)=\mathbb P(U_j\leq F(x))=F(x)$. [Independence of random variables](../../../../../../independent-random-variables.md) then gives the stated product [prior distribution](../../../../../../prior-probability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
