<h1 id="29k/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

At time $t$, immediate exercise is worth $(S_t-K)^+$, while waiting is worth the [European call option](../../../../../../european-call-option.md) price with remaining maturity $\tau=T-t$. The conditional version of part (iii) gives

$$
C(t,S_t)\geq S_t-e^{-r\tau}K.
$$

Under the standard Black-Scholes assumption $r\geq0$, this is at least $S_t-K$, while a call value is nonnegative. Hence $C(t,S_t)\geq(S_t-K)^+$, and the investor should wait until $T$; with $\sigma>0$ and $\tau>0$, waiting has strictly positive time value.

If negative interest rates are allowed, the unconditional instruction “wait” need not be correct. The exact decision is to exercise when

$$
(S_t-K)^+\geq S_t\Phi(d_+(\tau))-Ke^{-r\tau}\Phi(d_-(\tau)),
$$

and otherwise to continue.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
