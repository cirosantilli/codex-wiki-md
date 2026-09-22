<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use base-two logarithms throughout, so information and entropy are in bits. The [relative entropy](../../../../../../kullback-leibler-divergence.md) of classical probability distributions is

$$
D(p\|q)=\sum_{x:p(x)>0}p(x)\log_2\frac{p(x)}{q(x)}.
$$

Set $0\log_2(0/q)=0$; if $p(x)>0$ and $q(x)=0$, define the value to be $+\infty$. In the finite case, $\ln u\leq u-1$ gives

$$
\begin{aligned}
(\ln2)D(p\|q)
&=-\sum_{x\in\operatorname{supp}p}p(x)\ln\frac{q(x)}{p(x)}\\
&\geq\sum_{x\in\operatorname{supp}p}[p(x)-q(x)]
=1-q(\operatorname{supp}p)\geq0.
\end{aligned}
$$

Hence **$D(p\|q)\geq0$**, with equality exactly when $p=q$: equality in the logarithm inequality requires $q(x)=p(x)$ on the support, and equality in the last step leaves no mass outside it.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
