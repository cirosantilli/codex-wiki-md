<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [Sauer-Shelah lemma](../../../../../../sauer-shelah-lemma.md) says that a [hypothesis class](../../../../../../concept-class.md) of finite [VC dimension](../../../../../../vc-dimension.md) $d$ satisfies

$$
\boxed{\Pi_H(m)\leq\sum_{j=0}^{\min(d,m)}\binom mj.}
$$

In particular, for $m\geq d\geq1$,

$$
\Pi_H(m)\leq\left(\frac{em}{d}\right)^d.
$$

Here the [binomial coefficients](../../../../../../binomial-coefficient-split.md) count small subsets. One way to obtain the last inequality is to set $t=d/m\leq1$: since $t^j\geq t^d$ for $j\leq d$,

$$
t^d\sum_{j=0}^d\binom mj\leq\sum_{j=0}^d\binom mjt^j\leq(1+t)^m\leq e^{mt}=e^d.
$$

Thus finite [VC dimension](../../../../../../vc-dimension.md) replaces the unrestricted exponential number of labellings by a polynomial bound in the sample size.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Computational learning theory](../../../../computational-learning-theory-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
