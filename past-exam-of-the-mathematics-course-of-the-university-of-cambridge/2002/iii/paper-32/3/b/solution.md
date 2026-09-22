<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the stated cash dividend is the only dividend before maturity and [interest rates](../../../../../../interest-rate.md) are nonnegative. Before its ex-dividend date, compare exercise now with retaining the option until any later deterministic date $u<t_1$. There is no dividend between these dates, and retaining the option has value at least that of a European call expiring at $u$, namely at least $S_t-XB(t,u)$. This is at least the immediate in-the-money payoff, and is strictly larger with positive interest. Thus exercise earlier in the open pre-dividend interval is not optimal; the only possible dividend-induced early-exercise opportunity is the last cum-dividend instant, conventionally denoted $t_1-$.

At that instant write $S_-=S_{t_1-}$ and $S_+=S_--D$, the ex-dividend price. Immediate in-the-money exercise pays $S_--X$. Continuing across the dividend and retaining the call to maturity gives at least $S_+-XB(t_1,T)$, since no further dividend remains. Therefore continuation minus immediate exercise is bounded below by

$$
S_--D-XB(t_1,T)-(S_--X)=X(1-B(t_1,T))-D.
$$

Consequently the [dividend-date call-exercise criterion](../../../../../../dividend-date-call-exercise-criterion.md) is

$$
\boxed{D<X(1-B(t_1,T))\ \Longrightarrow\ \text{no beneficial early exercise before }T.}
$$

If the pre-dividend call is out of the money, exercising gives no benefit in the first place. After the dividend, part (a) excludes later early exercise. The comparison is a sufficient condition: failing it does not prove exercise is optimal, because continuation also includes put/time value not present in this lower bound.

The date convention matters. A dividend can make exercise just before the ex-dividend date optimal. Thus a literal assertion excluding $t_1-$ under all dividends would be false; the pre-dividend non-exercise argument excludes earlier dates, leaving this last cum-dividend opportunity to be tested. Further dividends would require separate tests at their own dates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
