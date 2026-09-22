<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $a>m$ and then $x>a$. By the assumptions on the [derivative](../../../../../../derivative.md) $\psi'$, there is a unique $\theta_x>0$ with $\psi'(\theta_x)=x$. Apply [exponential tilting](../../../../../../exponential-tilting.md) to each summand:

$$
\frac{d\mathbb P_{\theta_x}}{d\mathbb P}(y)
=e^{\theta_xy-\psi(\theta_x)}.
$$

Under the product tilted law, the variables remain [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) and have mean $x$. Hence the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) implies that, for every $0<\delta<x-a$,

$$
\mathbb P_{\theta_x}(|S_n/n-x|<\delta)\longrightarrow1.
$$

Changing measure on this event gives

$$
\mathbb P(S_n/n\geq a)
\geq e^{-n[\theta_x(x+\delta)-\psi(\theta_x)]}
\mathbb P_{\theta_x}(|S_n/n-x|<\delta).
$$

Therefore

$$
\liminf_{n\to\infty}\frac1n\log\mathbb P(S_n/n\geq a)
\geq-\psi^*(x)-\theta_x\delta.
$$

First let $\delta\downarrow0$ and then $x\downarrow a$. The [continuity of a convex function](../../../../../../continuity-of-a-convex-function.md) gives the lower bound $-\psi^*(a)$. The endpoint $a=m$ follows by letting $a\downarrow m$, while for $a<m$ the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) makes the probability tend to one. This proves the required lower bound.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
