<h1 id="8/c/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First restrict to [integers](../../../../../../integer-split.md) in the marginal supports: $2\leq i\leq12$ and $-5\leq j\leq5$. Their marginal [probabilities](../../../../../../probability.md) are positive. By part (i), a feasible joint pair identifies a unique ordered pair of rolls, so its joint [probability](../../../../../../probability.md) is $1/36$; an infeasible pair has joint [probability](../../../../../../probability.md) zero.

Put $a_i=6-|i-7|$ and $b_j=6-|j|$. If the two [events](../../../../../../event.md) were independent, a feasible pair would require

$$
\frac1{36}=\frac{a_i}{36}\frac{b_j}{36},\qquad\text{so }a_ib_j=36.
$$

Since $1\leq a_i,b_j\leq6$, equality forces $a_i=b_j=6$, hence $(i,j)=(7,0)$. But that pair is infeasible. An infeasible pair cannot give independence either, since its joint [probability](../../../../../../probability.md) is zero while the product of its positive marginal [probabilities](../../../../../../probability.md) is positive. Thus

$$
\boxed{\text{There are no independent pairs of these events within the two marginal supports}.}
$$

If all real values of $i,j$ are allowed literally, an impossible [event](../../../../../../event.md) is independent of every [event](../../../../../../event.md). The complete answer without a support restriction is therefore

$$
\boxed{\{X=i\}\text{ and }\{Y=j\}\text{ are independent iff }i\notin\{2,\ldots,12\}\text{ or }j\notin\{-5,\ldots,5\}.}
$$

## ↑ Ancestors (13)

1. [V](../v.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
