<h1 id="29j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the prescribed mean, $w_1-b$ has a [normal distribution](../../../../../../normal-distribution.md) with mean $d=m-b$ and standard deviation $\sigma$. Integrating its negative part gives the expected loss

$$
L(d,\sigma)=\sigma\varphi(d/\sigma)-d\Phi(-d/\sigma)\quad(\sigma>0),
$$

where $\varphi,\Phi$ are the standard normal density and distribution function. Differentiation at fixed $d$ yields $\partial L/\partial\sigma=\varphi(d/\sigma)>0$; the expression extends continuously to $\sigma=0$. Therefore **minimizing expected shortfall at a fixed mean chooses exactly the minimum-variance portfolio $\theta^*$** from part (a).

For $m\geq b$ it lies on the [mean-variance efficient frontier](../../../../../../efficient-frontier.md). If “efficient frontier” has its usual undominated meaning, the printed claim needs this qualification: for $m<b$, the same optimizer lies on the lower minimum-variance branch and is dominated by the all-bank point $(b,0)$. It still solves the fixed-mean problem, but is not efficient in that unconstrained comparison. If the term instead means the full fixed-mean minimum-variance boundary, the claim holds for every feasible $m$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
