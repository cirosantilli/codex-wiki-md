<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a given time write $p_i=P_i^t$ and $q_i=\alpha_ip_i$, the conditional probability that the next search succeeds if box $i$ is chosen. Compare two consecutive searches $i,j$, keeping the continuation after two failures fixed. Their expected costs up to that common continuation are

$$
C_{ij}=c_i+(1-q_i)c_j,
\qquad
C_{ji}=c_j+(1-q_j)c_i.
$$

The probability of reaching the common continuation is the same in either order. Moreover,

$$
C_{ij}\leq C_{ji}
\Longleftrightarrow
q_ic_j\geq q_jc_i
\Longleftrightarrow
\frac{\alpha_ip_i}{c_i}
\geq\frac{\alpha_jp_j}{c_j}.
$$

Repeated adjacent interchanges move a box with maximal index to the front without increasing expected cost; applying the same argument after every failure proves the [optimal index for Bayesian box search](../../../../../../optimal-index-for-bayesian-box-search.md) policy

$$
\boxed{\text{search a box maximizing }
\frac{\alpha_iP_i^t}{c_i}.}
$$

For completeness, after an unsuccessful search of box $i$, [Bayes' theorem](../../../../../../bayes-theorem.md) gives the posterior in the [Bayesian box search problem](../../../../../../bayesian-box-search-problem.md):

$$
P_i^{t+1}=\frac{(1-\alpha_i)P_i^t}{1-\alpha_iP_i^t},
\qquad
P_j^{t+1}=\frac{P_j^t}{1-\alpha_iP_i^t}\quad(j\ne i).
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
