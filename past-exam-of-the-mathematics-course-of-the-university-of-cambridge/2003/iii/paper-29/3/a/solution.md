<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Brownian first-passage time](../../../../../../brownian-first-passage-time.md) $T_a$ is finite [almost surely](../../../../../../almost-sure-convergence.md). Indeed the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives $\mathbb P(T_a\leq t)=2\mathbb P(B_t\geq a)\to1$ as $t\to\infty$. Continuity of the paths means the first passage to $x+y$ occurs after the first passage to $x$. By the [Strong Markov property](../../../../../../strong-markov-property.md), the process $B_{T_x+s}-x$ is an independent fresh [Brownian motion](../../../../../../brownian-motion-split.md). Thus $T_{x+y}-T_x$ has the same [probability distribution](../../../../../../probability-distribution.md) as $T_y$ and is independent of $T_x$. Taking the [Laplace transforms of nonnegative random variables](../../../../../../laplace-transform-of-a-nonnegative-random-variable.md) gives

$$
\boxed{\varphi_{x+y}(\lambda)=\varphi_x(\lambda)\varphi_y(\lambda).}
$$

For fixed $\lambda\geq0$, these transforms lie in $(0,1]$. Put $g(a)=-\log\varphi_a(\lambda)$. It is additive on positive arguments and nondecreasing, because the hitting times increase with the level. Writing $c(\lambda)=g(1)$, additivity gives $g(r)=rc(\lambda)$ for positive rational $r$, and rational upper and lower approximations then give $g(a)=ac(\lambda)$ for every $a>0$. Hence $\varphi_a(\lambda)=e^{-ac(\lambda)}$, with $c(\lambda)\geq0$.

The [Brownian scaling](../../../../../../brownian-scaling.md) identity $T_a\overset d=a^2T_1$ gives

$$
e^{-ac(\lambda)}=\varphi_1(a^2\lambda)=e^{-c(a^2\lambda)}.
$$

For $\lambda>0$, take $a=\sqrt\lambda$ in this relation with the transform parameter one. It follows that $c(\lambda)=C\sqrt\lambda$, where $C=c(1)\geq0$. At zero, finiteness of the hitting time gives $c(0)=0$. Thus $\boxed{\varphi_a(\lambda)=e^{-aC\sqrt\lambda}}$, with the constant determined in part (b).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
