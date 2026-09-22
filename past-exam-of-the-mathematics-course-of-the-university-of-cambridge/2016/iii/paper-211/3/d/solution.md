<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $h$ be the [stock](../../../../../../stock.md) holding and let $c$ be the initial cost, so the cash holding is $b=c-10h$. Terminal [portfolio](../../../../../../investment-portfolio.md) wealth at [stock](../../../../../../stock.md) price $s$ is $c+h(s-10)$. Dominating the [European call option](../../../../../../european-call-option.md) payoff at the three possible prices gives

$$
c-h\geq0,\qquad c\geq0,\qquad c+h\geq1.
$$

Adding the two endpoint inequalities yields $2c\geq1$. Equality is attained by $h=1/2$ and $c=1/2$, which imply $b=-9/2$. The corresponding terminal wealth is $0,1/2,1$ at $s=9,10,11$, respectively, compared with the required payoff $0,0,1$. **The cheapest super-replication strategy is**

$$
\boxed{\text{hold }\frac12\text{ share and }-\frac92\text{ units of cash};\qquad c_{\min}=\frac12.}
$$

The middle-state excess shows why this is [superhedging](../../../../../../superhedging.md) rather than exact [claim replication](../../../../../../claim-replication.md). The endpoint bound proves global minimality, without relying on the physical state [probabilities](../../../../../../probability.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
