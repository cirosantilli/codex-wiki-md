<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In each trial the presence indicators of $A$ and $B$ are independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md), with probabilities $p$ and $r$. Independence across trials makes their two entire indicator sequences independent. Let $N$ be the number of trials before the first $A$; then $N\sim\operatorname{Geom}_0(p)$. Among these $N$ preceding trials, the $B$ indicators are independent with probability $r$.

Thus the count is the [random sum](../../../../../../random-sum.md) from part [i](../b/i.md), and

$$
\boxed{\text{count}\sim\operatorname{Geom}_0\!\left(\frac p{p+(1-p)r}\right).}
$$

An $AB$ outcome on the stopping trial contributes nothing, because the question counts only outcomes strictly before the first $A$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
