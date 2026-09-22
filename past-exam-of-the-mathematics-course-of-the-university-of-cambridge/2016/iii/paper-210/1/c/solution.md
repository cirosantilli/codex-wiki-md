<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $a=\sqrt{n\log d/2}$ and $b=\sqrt{n\log(1/\delta)/2}$. Use the [scan statistic](../../../../../../scan-statistic.md) $C$ and the [statistical hypothesis testing](../../../../../../statistical-hypothesis-test.md) rule

$$
\boxed{\psi=\mathbf1_{\{C>n\varepsilon+a+b\}}.}
$$

The [union bound](../../../../../../boole-s-inequality.md) and the [Hoeffding inequality](../../../../../../hoeffding-inequality.md) give $P_0(\psi=1)\leq d\exp[-2(a+b)^2/n]\leq\delta$, since $(a+b)^2\geq a^2+b^2$. Conditional on index $j$, accepting the [null hypothesis](../../../../../../null-hypothesis.md) implies $c_j\leq n\varepsilon+a+b$. The assumed separation gives $n\pi(1-\varepsilon)>a+2b$, so this threshold lies more than $b$ below the alternative [expected value](../../../../../../expected-value.md) $np_1$. The lower-tail [Hoeffding inequality](../../../../../../hoeffding-inequality.md) therefore gives $Q_j(\psi=0)\leq\delta$. Averaging the conditional error over the [mixture model](../../../../../../mixture-model.md) gives $P_1(\psi=0)\leq\delta$ as well.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
