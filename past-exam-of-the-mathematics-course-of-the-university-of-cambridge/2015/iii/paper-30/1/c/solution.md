<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K=\sup_T\mathbb E[e^{M_T/2}]<\infty$, with $T$ ranging over finite stopping times. To locate the [half-threshold for the exponential-martingale Hölder bound](../../../../../../half-threshold-for-the-exponential-martingale-holder-bound.md), put $u=\sqrt{pq}>\sqrt q$. Since $u(u-1)$ is increasing for $u>1$,

$$
C(p,q)>\frac{q-\sqrt q}{q-1}
=\frac{\sqrt q}{\sqrt q+1}>\frac12.
$$

On the other hand, taking $q=1+\varepsilon$ and $p=1+\varepsilon^2$ gives $C(p,q)\to1/2$ as $\varepsilon\downarrow0$. Hence

$$
\boxed{\inf_{p,q>1}C(p,q)=\frac12.}
$$

Fix $0<a<1$. Choose $p,q>1$ with $aC(p,q)<1/2$, and put $\lambda=2aC(p,q)\in(0,1)$. Part (a) and the [Jensen inequality](../../../../../../jensen-s-inequality.md) give, for every finite stopping time,

$$
\begin{aligned}
\mathbb E[\mathcal E(aM)_T^p]
&\leq\bigl(\mathbb E[(e^{M_T/2})^\lambda]\bigr)^{(q-1)/q}\\
&\leq K^{\lambda(q-1)/q}.
\end{aligned}
$$

Thus the entire stopped family has a uniform $L^p$ bound for some $p>1$. By [uniform integrability from an Lp bound](../../../../../../uniform-integrability-from-an-lp-bound.md), it is [uniformly integrable](../../../../../../uniform-integrability.md).

To check that this [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md), stop it by a [localizing sequence](../../../../../../localizing-sequence.md). At each fixed time the stopped variables are [uniformly integrable](../../../../../../uniform-integrability.md) by the same bound; taking limits in their conditional [martingale](../../../../../../martingale-split.md) identities proves the unstopped identity. The uniform bound over all finite stopping times then makes it a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md), with terminal expectation one. Therefore

$$
\boxed{\mathcal E(aM)\text{ is a uniformly integrable martingale for every }0<a<1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
