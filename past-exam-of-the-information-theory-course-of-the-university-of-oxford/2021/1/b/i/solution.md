<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [probability mass functions](../../../../../probability-mass-function.md) on the [finite alphabet](../../../../../finite-alphabet.md), take [logarithms](../../../../../logarithm.md) to base two and define the [relative entropy](../../../../../kullback-leibler-divergence.md) by

$$
\boxed{D(q\|p)=\sum_{i=1}^mq_i\log_2\frac{q_i}{p_i}.}
$$

A term with $q_i=0$ is zero, including $p_i=0$; a term with $q_i>0=p_i$ is $+\infty$. Fix $p_i>0$ and write $f_i(t)=t\log_2(t/p_i)$. For $t>0$,

$$
f_i''(t)=\frac1{t\ln2}>0,\qquad \lim_{t\downarrow0}f_i(t)=0.
$$

Thus $f_i$ is a [convex function](../../../../../convex-function.md) on $[0,\infty)$ by continuous extension to zero. For $0\leq\lambda\leq1$, applying this scalar [convexity](../../../../../convex-function.md) to each coordinate and summing proves

$$
D(\lambda q+(1-\lambda)r\|p)\leq\lambda D(q\|p)+(1-\lambda)D(r\|p).
$$

If $p$ has zero coordinates, the finite-valued domain consists of [probability mass functions](../../../../../probability-mass-function.md) supported on $\{i:p_i>0\}$; it is convex and the same proof applies there. Outside that domain the right side is infinite whenever an offending [probability mass function](../../../../../probability-mass-function.md) has a positive mixture weight, so the extended-valued [convexity](../../../../../convex-function.md) assertion still holds. At mixture weights zero or one the inequality is an identity, without needing the expression $0\cdot\infty$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
