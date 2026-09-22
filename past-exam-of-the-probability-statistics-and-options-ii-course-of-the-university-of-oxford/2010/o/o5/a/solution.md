<h1 id="o/o5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a rejection function $\varphi(x)\in[0,1]$, its [power](../../../../../power-function-of-a-statistical-test.md) is $\beta(\theta)=\mathbb E_\theta\varphi(X)$. A test has level at most $\alpha$ if $\sup_{\theta\in H_0}\beta(\theta)\le\alpha$; its size is that supremum. In a simple null the significance probability is just the rejection probability under that null.

For two simple hypotheses with joint sample [densities](../../../../../probability-density-function.md) $f_0,f_1$, the [Neyman–Pearson lemma](../../../../../neyman-pearson-lemma.md) states that a test rejecting where $f_1>kf_0$, accepting where $f_1<kf_0$, and randomizing if necessary on equality to have size $\alpha$, is most powerful among level-$\alpha$ tests. Let $\varphi_*$ be that test and $\varphi$ any competitor. Pointwise,

$$
(\varphi_*-\varphi)(f_1-kf_0)\ge0.
$$

Integration gives

$$
\int(\varphi_*-\varphi)f_1\ge k\int(\varphi_*-\varphi)f_0\ge0,
$$

since $k\ge0$, the first test has size $\alpha$, and the other has size at most $\alpha$. This proves the claimed [power](../../../../../power-function-of-a-statistical-test.md) bound, allowing null-[density](../../../../../probability-density-function.md)-zero regions as well. Equality implies agreement away from the [likelihood](../../../../../likelihood-function.md)-ratio boundary, up to null sets, when the inequalities are strict.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
