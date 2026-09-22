<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P_0,P_1$ be simple hypotheses with densities $p_0,p_1$ (their [Radon-Nikodym derivatives](../../../../../../radon-nikodym-derivative.md)) relative to a common dominating [measure](../../../../../../measure.md). A possibly randomised [statistical test](../../../../../../statistical-test.md) is a measurable function $\varphi\in[0,1]$; its [size of a statistical test](../../../../../../size-of-a-statistical-test.md) is $E_0\varphi$ and its [statistical power](../../../../../../statistical-power.md) is $E_1\varphi$. The [Neyman-Pearson lemma](../../../../../../neyman-pearson-lemma.md) says that a [likelihood ratio](../../../../../../likelihood-ratio.md) threshold test

$$
\varphi_*(x)=\begin{cases}1,&p_1(x)>c p_0(x),\\0,&p_1(x)<c p_0(x),\\\gamma(x),&p_1(x)=c p_0(x),\end{cases}\qquad c\geq0,
$$

chosen to have size $\alpha$, is a [most powerful test](../../../../../../most-powerful-test.md) among tests of size at most $\alpha$. A constant randomisation on the equality set suffices to reach the required size; sets where $p_0=0<p_1$ are always rejected. For $0<\alpha<1$, a quantile of the [likelihood ratio](../../../../../../likelihood-ratio.md) under $P_0$ gives such a threshold. If the threshold is zero, randomisation where $p_1=0$ may be needed to use the remaining size. At $\alpha=0$, one can reject only a $P_0$-null set and optimally reject the part supporting $P_1$; at $\alpha=1$, always reject.

For the proof, every competing $\varphi$ satisfies

$$
(\varphi_* -\varphi)(p_1-cp_0)\geq0
$$

pointwise: the signs agree off the equality set, where the product is zero. Integrating gives

$$
E_1\varphi_*-E_1\varphi\geq c(E_0\varphi_*-E_0\varphi)\geq0.
$$

Thus **the likelihood-ratio threshold test has maximum power at the stated level**. If $c>0$, a competing most-powerful test must have size $\alpha$ and agree with $\varphi_*$ off the equality set, apart from sets null for $P_0+P_1$; both inequalities must then be equalities. For $c=0$, equal size is not necessary for optimality, because changing decisions where $p_1=0$ does not affect power. These qualifications account for ties and singular supports rather than assuming all densities are strictly positive.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
