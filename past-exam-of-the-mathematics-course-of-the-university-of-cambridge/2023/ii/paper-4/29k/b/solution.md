<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now $R=1+r=9/8$. The local [risk-neutral up probabilities](../../../../../../risk-neutral-probability-in-a-binomial-market.md) solve $RS=qS_u+(1-q)S_d$. They are

$$
q_0=\frac{(9/8)5-4}{6-4}=\frac{13}{16},
\qquad
q_u=\frac{(9/8)6-5}{7-5}=\frac78,
\qquad
q_d=\frac{(9/8)4-3}{5-3}=\frac34.
$$

The terminal payoff of the [European put option](../../../../../../european-put-option.md) with strike $5$ is $0,0,2$ at stock prices $7,5,3$. [Backward option pricing](../../../../../../backward-option-pricing.md) gives time-one values

$$
V_u=0,
\qquad
V_d=R^{-1}\left(\frac14\cdot2\right)=\frac49,
$$

and hence

$$
V_0=R^{-1}\left(\frac{3}{16}\frac49\right)=\boxed{\frac{2}{27}}.
$$

The first-period stock holding in the [replicating portfolio in a binomial market](../../../../../../replicating-portfolio-in-a-binomial-market.md) is

$$
\Delta_0=\frac{V_u-V_d}{6-4}=-\frac29.
$$

**Thus the hedge initially shorts $2/9$ of a share.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
