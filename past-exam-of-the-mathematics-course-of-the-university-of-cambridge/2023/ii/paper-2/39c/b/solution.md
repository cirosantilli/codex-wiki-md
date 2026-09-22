<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $a$ denote the bubble size, $U$ its speed, and $\operatorname{Re}=Ua/\nu\gg1$ the [Reynolds number](../../../../../../reynolds-number.md). Outside a thin [boundary layer](../../../../../../boundary-layer.md), inertia dominates and the flow is an [irrotational flow](../../../../../../irrotational-flow.md) with velocity scale $U$ and strain scale $U/a$. Its viscous dissipation has order

$$
\mathcal D_{\rm outer}
\sim \mu\left(\frac Ua\right)^2a^3
\sim\mu U^2a
$$

in three dimensions.

The boundary-layer thickness is

$$
\delta\sim\left(\frac{\nu a}{U}\right)^{1/2}
=a\operatorname{Re}^{-1/2}.
$$

For a clean bubble the [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) prescribes tangential stress rather than tangential velocity. The outer flow already has tangential strain of order $U/a$, so cancelling that stress requires a velocity correction of only

$$
\Delta u\sim\frac Ua\delta,
$$

not a correction of order $U$. Its gradient remains $O(U/a)$, and its boundary-layer dissipation is

$$
\mathcal D_{\rm layer}
\sim\mu\left(\frac Ua\right)^2a^2\delta
\sim\mathcal D_{\rm outer}\frac\delta a,
$$

which is asymptotically smaller.

In steady translation, the drag power $DU$ balances viscous dissipation. The leading estimate therefore follows from the known outer flow alone:

$$
\boxed{D\sim\frac{\mathcal D_{\rm outer}}U\sim\mu Ua}
$$

in three dimensions. This is the [dissipation estimate for high-Reynolds-number bubble drag](../../../../../../dissipation-estimate-for-high-reynolds-number-bubble-drag.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
