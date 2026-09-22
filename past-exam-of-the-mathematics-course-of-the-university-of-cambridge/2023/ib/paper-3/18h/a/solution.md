<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A possibly randomized test is a function $\varphi(X)\in[0,1]$, interpreted as the conditional probability of rejecting $H_0$. Its [power function](../../../../../../power-function-of-a-statistical-test.md) is

$$
\pi_\varphi(\theta)=\mathbb E_\theta[\varphi(X)].
$$

It has size at most $\alpha$ when

$$
\sup_{\theta\in\Theta_0}\pi_\varphi(\theta)\leq\alpha.
$$

Such a test is a [uniformly most powerful test](../../../../../../uniformly-most-powerful-test.md) of size $\alpha$ if, for every other test $\psi$ of size at most $\alpha$,

$$
\pi_\varphi(\theta)\geq\pi_\psi(\theta)
\qquad\text{for every }\theta\in\Theta_1.
$$

**Thus one test maximizes power simultaneously at every parameter value in the alternative.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
