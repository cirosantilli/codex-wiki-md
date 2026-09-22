<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $K'=K(1+r)^{t_0-T}$. At the choice time,

$$
 \max(c_{t_0},p_{t_0})=c_{t_0}+(K'-S_{t_0}^1)^+.
$$

Buy a [European call option](../../../../../../european-call-option.md) of strike $K$ and maturity $T$, together with a [European put option](../../../../../../european-put-option.md) of strike $K'$ and maturity $t_0$. If the call is selected, the short-maturity put expires worthless. If the put is selected, sell the call and combine its value with the short-maturity put's cash payment; [put-call parity](../../../../../../put-call-parity.md) makes this exactly enough to buy the maturity-$T$ put. This self-financing replication proves

$$
\boxed{\pi(C(K,t_0,T))=\pi(EC(K,T))+\pi(EP(K(1+r)^{t_0-T},t_0)).}
$$

It requires tradability of the priced options at the choice time, but not completeness of every other market claim. The identity also covers $t_0=0$ and $t_0=T$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
