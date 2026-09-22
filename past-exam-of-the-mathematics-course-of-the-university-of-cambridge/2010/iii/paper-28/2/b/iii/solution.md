<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix times $t_1,\ldots,t_d\in[0,1]$, and set

$$
V_k=(\mathbf1_{\{X_k\leq t_j\}}-t_j)_{j=1}^d.
$$

These are iid bounded centred [random vectors](../../../../../../../random-vector.md), and

$$
(Z_n(t_j))_{j=1}^d=n^{-1/2}\sum_{k=1}^nV_k.
$$

Their covariance matrix is

$$
C_{ij}=\mathbb P(X_1\leq\min(t_i,t_j))-t_it_j
=\min(t_i,t_j)-t_it_j.
$$

We prove the required [central limit theorem](../../../../../../../central-limit-theorem.md) calculation explicitly. For $u\in\mathbb R^d$, the scalar $u\cdot V_1$ is bounded, has mean zero and second moment $u^TCu$. The Taylor expansion of the exponential, with its uniformly bounded cubic remainder, gives

$$
\mathbb E e^{iu\cdot V_1/\sqrt n}
=1-\frac{u^TCu}{2n}+O_u(n^{-3/2}).
$$

Independence implies that the [characteristic function](../../../../../../../characteristic-function.md) of the sum vector is the $n$th power of this expression, so it tends to $\exp(-u^TCu/2)$. This is the [characteristic function](../../../../../../../characteristic-function.md) of a centred [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) with covariance $C$. The [Lévy continuity theorem](../../../../../../../levy-continuity-theorem.md) states that convergence of characteristic functions to a characteristic function continuous at zero gives [convergence in distribution](../../../../../../../convergence-in-distribution.md); apply it here.

By part (ii), the corresponding [Brownian bridge](../../../../../../../brownian-bridge.md) vector has exactly this covariance and mean. Therefore

$$
\boxed{(Z_n(t_1),\ldots,Z_n(t_d))\ \xrightarrow{\ d\ }\ (Z_{t_1},\ldots,Z_{t_d}).}
$$

Repeated times or the endpoint times may make $C$ singular; the characteristic-function argument still applies. This proves every [finite-dimensional distribution](../../../../../../../finite-dimensional-distribution.md) convergence requested, the uniform case of the [Finite-dimensional Brownian bridge limit of an empirical distribution process](../../../../../../../finite-dimensional-brownian-bridge-limit-of-an-empirical-distribution-process.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
