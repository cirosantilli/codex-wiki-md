<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $0<\pi<1$, let $\delta_\pi$ be the [Bayes classifier](../../../../../../bayes-classifier.md) with class-zero prior $\pi$, and define its two class-conditional error probabilities by

$$
e_0(\pi)=\mathbb P_0(\delta_\pi(X)=1),
\qquad
e_1(\pi)=\mathbb P_1(\delta_\pi(X)=0).
$$

Writing the [likelihood ratio](../../../../../../likelihood-ratio.md) as $L=f_1/f_0$, the rule chooses class one when

$$
L(x)\geq\frac\pi{1-\pi}.
$$

The Gaussian likelihood-ratio level sets have probability zero, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) shows that $e_0$ and $e_1$ depend continuously on $\pi$. As $\pi\downarrow0$, the threshold tends to zero and the classifier chooses class one almost surely, giving

$$
(e_0(\pi),e_1(\pi))\longrightarrow(1,0).
$$

As $\pi\uparrow1$, it chooses class zero almost surely, giving the opposite limit $(0,1)$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) therefore provides $\pi^*\in(0,1)$ such that

$$
e_0(\pi^*)=e_1(\pi^*)=:r.
$$

The rule $\delta_{\pi^*}$ is an [equalizer rule](../../../../../../equalizer-rule.md) with worst-case risk $r$. For any classifier $\delta$,

$$
\begin{aligned}
\max\{R_0(\delta),R_1(\delta)\}
&\geq \pi^*R_0(\delta)+(1-\pi^*)R_1(\delta)\\
&\geq \pi^*e_0(\pi^*)+(1-\pi^*)e_1(\pi^*)=r,
\end{aligned}
$$

because $\delta_{\pi^*}$ minimizes the integrated risk for its prior. Hence $\delta_{\pi^*}$ is a [minimax decision rule](../../../../../../minimax-decision-rule.md), as summarized by the [minimax Gaussian Bayes classifier from equal class errors](../../../../../../minimax-gaussian-bayes-classifier-from-equal-class-errors.md).

The prior is indeed [least favorable](../../../../../../least-favorable-prior.md). Its [Bayes risk](../../../../../../bayes-risk.md) is $r$, while for any other prior $q$ the Bayes risk is at most the integrated risk of the same equalizer rule $\delta_{\pi^*}$, namely

$$
q r+(1-q)r=r.
$$

**Thus no prior has larger Bayes risk.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
