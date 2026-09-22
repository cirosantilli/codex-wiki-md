<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $\sigma\ne0$ and the usual [Brownian filtration](../../../../../../brownian-filtration.md), so the single-risky-asset market is a [complete market](../../../../../../complete-market.md). With [market price of risk](../../../../../../market-price-of-risk.md) $\kappa=(\mu-r)/\sigma$, the normalized [state-price density](../../../../../../state-price-density.md) is

$$
\boxed{\zeta_t=\exp[-rt-\kappa W_t-\tfrac12\kappa^2t]},\qquad
d\zeta_t=-r\zeta_t\,dt-\kappa\zeta_t\,dW_t.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) shows that $\zeta_tw_t$ is a [local martingale](../../../../../../local-martingale.md) for a [self-financing portfolio](../../../../../../self-financing-portfolio.md). For nonnegative admissible wealth it is a [supermartingale](../../../../../../supermartingale.md), yielding the [state-price budget constraint](../../../../../../state-price-budget-constraint.md)

$$
\mathbb E[\zeta_Tw_T]\leq w.
$$

Every integrable nonnegative terminal claim with equality is attainable in the [complete market](../../../../../../complete-market.md), by the [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md). Its wealth process is $w_t=\zeta_t^{-1}\mathbb E[\zeta_TX\mid\mathcal F_t]\geq0$.

The [Inada conditions](../../../../../../inada-conditions.md) $u'(0+)=\infty$ and $u'(\infty)=0$, together with strict [concavity](../../../../../../concave-function.md), make $I=(u')^{-1}$ a decreasing map from $(0,\infty)$ onto $(0,\infty)$. Pointwise optimization of $u(x)-y\zeta_Tx$ gives **the optimal terminal wealth**

$$
\boxed{w_T^*=I(y\zeta_T),\qquad
\mathbb E[\zeta_TI(y\zeta_T)]=w,}
$$

with scalar multiplier $y>0$. The question assumes a multiplier giving the required budget; utility expectations must also be well defined.

For any admissible terminal wealth $X$, the supporting-line inequality for a [concave function](../../../../../../concave-function.md) gives

$$
u(X)-u(w_T^*)\leq u'(w_T^*)(X-w_T^*)
=y\zeta_T(X-w_T^*).
$$

Taking expectations and using the [state-price budget constraint](../../../../../../state-price-budget-constraint.md) proves **optimality**:

$$
\boxed{\mathbb Eu(X)\leq\mathbb Eu(w_T^*)+
y(\mathbb E[\zeta_TX]-w)\leq\mathbb Eu(w_T^*).}
$$

Strict [concavity](../../../../../../concave-function.md) makes the optimal terminal wealth unique up to almost-sure equality.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
