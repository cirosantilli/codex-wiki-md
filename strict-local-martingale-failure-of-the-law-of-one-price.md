# Strict local martingale failure of the law of one price

↑ **Parent:** [Law of one price](law-of-one-price.md)

Fix $T>0$, let $X$ be [Brownian motion](brownian-motion-split.md), and let $\tau=\inf\{u:X_u=-1\}$. Set $q(t)=t/(T-t)$ for $t<T$ and

$$
B_t=1,\qquad S_t=2+X_{q(t)\wedge\tau}\quad(t<T),\qquad S_T=1.
$$

The hitting time is finite almost surely, so each price path reaches one before $T$ and stays there. Stopping additionally on hitting $n+2$ makes the [stock](stock.md) price a bounded [martingale](martingale-split.md); these stopping times increase to $T$. Hence $S$ is a positive [local martingale](local-martingale.md), and the original probability measure is an [equivalent local martingale measure](equivalent-local-martingale-measure.md), excluding admissible [arbitrage](arbitrage.md). Nevertheless $S_T=B_T$ while $S_0=2\ne1=B_0$. The zero-cost short-stock/long-two-cash [portfolio](investment-portfolio.md) has terminal gain one but wealth $2-S_t$, which has no deterministic lower bound. It is not admissible, resolving the apparent contradiction.

## ↑ Ancestors (7)

1. [Law of one price](law-of-one-price.md)
2. [Arbitrage](arbitrage.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
