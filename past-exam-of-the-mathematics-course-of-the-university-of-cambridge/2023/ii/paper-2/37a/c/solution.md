<h1 id="37a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Several [microstates](../../../../../../microstate.md) can have the same extension. If $g(l)$ denotes their [state degeneracy](../../../../../../state-degeneracy.md), grouping equal terms in the state sum gives

$$
Z=\sum_i e^{\tau l_i}
=\boxed{\sum_l g(l)e^{\tau l}}.
$$

For the [one-dimensional freely jointed chain](../../../../../../one-dimensional-freely-jointed-chain.md), a [macrostate](../../../../../../macrostate.md) with $n_+$ positive links and $n_-=n-n_+$ negative links has

$$
l=(n_+-n_-)a,
\qquad
g(l)=\frac{n!}{n_+!n_-!}.
$$

Hence

$$
Z=\sum_{n_+=0}^n
\frac{n!}{n_+!n_-!}
(e^{\tau a})^{n_+}(e^{-\tau a})^{n_-}.
$$

The [binomial theorem](../../../../../../binomial-theorem.md) now gives the [fixed-tension partition function of a one-dimensional chain](../../../../../../fixed-tension-partition-function-of-a-one-dimensional-chain.md)

$$
\boxed{Z=(e^{\tau a}+e^{-\tau a})^n
=(2\cosh(\tau a))^n.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [37A](../../37a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
